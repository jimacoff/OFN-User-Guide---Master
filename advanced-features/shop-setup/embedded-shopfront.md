# Embedded Shopfront

This feature lets users who have Abukem shopfronts embed their shop into their own website. This gives customers a more fluid experience and avoids the need to redirect them between multiple websites. It also allows users to retain some of their visual branding in the shop. When you embed your Abukem shop in your own site, your Abukem based shop will remain, so customers can choose where they want to shop. This page details the requirements for using embedded shopfronts and the steps to get it setup. There is also a link to an example of how an embedded shopfront will look.

## Requirements

### Platforms

This feature is relatively new, and we’re still testing it out, but it should work on any kind of website, as long as you can add custom html to the page where you want the shop. Whether your website is supported by WordPress, Squarespace, Wix or another platform, it should be able to be setup to embed your shopfront.

Below are some platform specific resources:

Squarespace lets you ‘add customer html’ via their “codeblocks” – see here.

#### Security

Because Abukem is an eCommerce platform, and handles monetary transactions, it has a higher security requirement than text only websites. Therefore, you’ll need to setup SSL/TLS on the website you want to embed your Abukem shop into if you haven’t already.

You can get such a security certificate for free from [Let’s Encrypt](https://letsencrypt.org/) or for around $10-$30 for a paid service.

### Abukem E-Maeket Shop

Of course, the last requirement is that you have a shop setup on Abukem. You’ll need to know your shop’s Abukem url in the setup steps below.

Getting setup

**1\) Contact your local Abukem team**

First of all, you’ll need to [contact your local Abukem team](https://abukem.com/contact/) and let them know that you want to embed your Abukem shop in your own website. You’ll need to provide them with your external domain. E.g. happyhenfarm.com so they can grant permission for your website to communicate with Abukem.

**2\) Adding Custom HTML to your website**

Embedding your shop is as simple as inserting a line of code into your website. This is the line of html that you should insert into the page where you want the shop:

```text
<iframe src=" https://abukem.com/happy-hens-farm/shop?embedded_shopfront=true"style="width:100%;min-height:35em"></iframe>
```

In the html above make sure to replace ‘happy-hens-farm’ with your shop’s unique OFN permalink.

Once you’ve done this, you should see your Abukem shopfront appear on your webpage.

**3\) Styling**

Depending on the styling of your website you may need to add some CSS tweaks. They may be needed to avoid having two scroll bars, and to make sure the length and width of the embedded shop looks visually appealing. Make sure to test the display of your embedded shop on a mobile device. If the mobile display is misbehaving you may need further CSS tweaks. The tweaks required will be different for every website, but your website administrator should be able to help you.

**Example**

We have setup an [example of an embedded shop](https://abukem.com/user-guide/advanced-features/demo-embedded-shop/) for you to look at and play with.

## Instructions for Customers

### Cookies

Most people have cookies enabled on their web browsers. But if a customer doesn’t enable cookies they won’t be able to shop in the embedded shop. The error message they’ll see is shown below. Note that they can shop at the version of your shop hosted by OFN without needing cookies enabled.

![](../../.gitbook/assets/ofn-cookies-embedded-shopfront.bin)

