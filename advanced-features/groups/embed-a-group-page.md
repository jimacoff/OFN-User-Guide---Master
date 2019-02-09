# Embed a Group Page

This feature lets you embed a group page into a website external to Abukem. This lets you use the Abukem group director tool on your own website. This page details the requirements for embedding a group page, and the steps to set it up. There is also an example of how an embedded group may look.

## Requirements

### Platform

This feature is relatively new, and we’re still testing it out, but it should work on any kind of website, **as long as you can add custom html** to the page where you want the group page. Whether your website is suported by WordPress, Squarespace, Wix or another platform, it should be able to be setup to embed your group page.

Below are some platform specific resources:

* Squarespace lets you ‘add customer html’ via their “codeblocks” –[see here](https://support.squarespace.com/hc/en-us/articles/206543167).

### Security

Because Abukem is an eCommerce platform, and handles monetary transactions, it has a higher security requirement than text only websites. Therefore, you’ll need to setup SSL/TLS on the website you want to embed your group page into if you haven’t already.

You can get such a security certificate for free from [Let’s Encrypt](https://letsencrypt.org/) for around $10-$30 for a paid service.

### Abukem Group page

Of course, the last requirement is that you have a group page setup on Abukem. You’ll need to know your group page’s Abukem url in the setup steps below.

## Getting setup

**1\) Contact your local Abukem team**

First of all, you’ll need to contact [your local Abukem team](https://abukem.com/ofn-local/), and let them know that you want to embed your Abukem group page in your own website. You’ll need to provide them with your external domain. E.g. freerange.com.au so they can grant permission for your website to communicate with Abukem.

**2\) Adding Custom HTML to your website**

Embedding your shop is as simple as inserting a line of code into your website. This is the line of html that you should insert into the page where you want the shop:

```text
<iframe src="/groups/flavour-crusader?embedded_shopfront=true"style="width:100%;min-height:35em"></iframe>
```

In the html above make sure to replace ‘flavour-crusader’ with your shop’s unique Abukem permalink.

Once you’ve done this, you should see your Abukem group page appear on your webpage.

**3\) Styling**

Depending on the styling of your website you may need to add some CSS tweaks. They may be needed to avoid having two scroll bars, and to make sure the length and width of the embedded group page looks visually appealing. Make sure to test the display of your group page on a mobile device as well. If the mobile display is misbehaving you may need further CSS tweaks. The tweaks required will be different for every website, but your website administrator should be able to help you.


## Instructions for Visitors

### Cookies

Most people have cookies enabled on their web browsers. But if a visitor doesn’t enable cookies they may not be able to view the embedded group.

![](../../.gitbook/assets/cookies.png)

