**Date Updated:** 2024-03-12T02:03:37.000Z

### More Tutorials from the Community

<https://youtu.be/Xd0eMUbxpr4>

https://youtu.be/Ea8JWlEKfGw

[](https://youtu.be/XgxEb7F7cIk)[https://youtu.be/XgxEb7F7cIk ](https://youtu.be/XgxEb7F7cIk​​)

  
While setting up SaaS in currencies other than USD can be slightly more tedious, it is indeed possible. Many agencies have successfully expanded their SaaS business internationally. This article will guide you through a proven and scalable setup process.
  
  
**TABLE OF CONTENTS**

* [Can I sell SaaS in non-USD currencies? ](#Can-I-sell-SaaS-in-non-USD-currencies?%C2%A0)
* [But when I create SaaS product they are always in USD. How can I change that?](#But-when-I-create-SaaS-product-they-are-always-in-USD.-How-can-I-change-that?)
* [My SaaS Configurator still shows USD. Is that a problem?](#My-SaaS-Configurator-still-shows-USD.-Is-that-a-problem?)
* [How can I start selling SaaS in this new currency?](#How-can-I-start-selling-SaaS-in-this-new-currency?)
* [What happens behind the scenes?](#What-happens-behind-the-scenes?)
* [But I want to use my funnel to sell this instead of Checkout links. How can I do that?](#But-I-want-to-use-my-funnel-to-sell-this-instead-of-Checkout-links.-How-can-I-do-that?)  
   * [How can I import my modified SaaS products and prices to the sub-account (location) I want to use for selling SaaS?](#How-can-I-import-my-modified-SaaS-products-and-prices-to-the-sub-account-%28location%29-I-want-to-use-for-selling-SaaS?)
* [What about the wallet recharges (credits)?](#What-about-the-wallet-recharges-%28credits%29?)
  
  
Native support for selling SaaS sub-accounts in currencies other than the USD will be available soon. **Until that time this workaround should work for all our SaaS agencies.**

  
# Can I sell SaaS in non-USD currencies? 

Yes, you can. By following the workaround detailed in this document, our SaaS agencies can sell SaaS in almost any currency supported by Stripe. [Click here](https://stripe.com/docs/currencies) to check which currencies Stripe supports based on your business country.

  
# But when I create SaaS product they are always in USD. How can I change that?

Initially, create your SaaS products in USD using the SaaS Configurator.

  
![](https://s3.amazonaws.com/cdn.freshdesk.com/data/helpdesk/attachments/production/155010056534/original/aiz-Ofx7jvEArutcHKrHitdG6x-8YDwjbg.png?1697198140)
  
  
Then login to your Stripe account and the products will look like this

  
![](https://s3.amazonaws.com/cdn.freshdesk.com/data/helpdesk/attachments/production/155009970166/original/3qCemDIge-T1k0l2NTdUQaqBAuDM-fwkOA.png?1697122069)

  
Now edit the prices and change the currency in your desired currency. In this in example I will be using USD.

  
![](https://s3.amazonaws.com/cdn.freshdesk.com/data/helpdesk/attachments/production/155009971637/original/GhdkCyVKk4LiWBOrT5iimckFdLTj1Eb1TQ.png?1697122864)

  
Now your Stripe products will be in the currency of your choice instead of USD. It should look like this

  
![](https://s3.amazonaws.com/cdn.freshdesk.com/data/helpdesk/attachments/production/155009970906/original/UsxS3aGtvlwCjHxrP3ShXhaz2nqvNcsd7A.png?1697122455)

  
 Repeat this process for all your SaaS products and prices.
  
  
# My SaaS Configurator still shows USD. Is that a problem?

 No, it's not. While the SaaS Configurator in your HighLevel agency view will continue to display products and prices in USD, the currency set in Stripe takes precedence. The currency onside Stripe overrides the currency in the SaaS Configurator. ![](https://s3.amazonaws.com/cdn.freshdesk.com/data/helpdesk/attachments/production/155010056771/original/KCbFist1lK0cA4DKg6_tlwrMWijYeuGL-g.png?1697198239)

  
# How can I start selling SaaS in this new currency?

You can start by generating payment links for your SaaS products.
  
  
The checkout will then reflect your chosen currency instead of USD.

![](https://s3.amazonaws.com/cdn.freshdesk.com/data/helpdesk/attachments/production/155010056868/original/HiF5MUQjo8_Cvw8IvBuiICfWqSHvRajAog.png?1697198304)

As you can see the checkout would be in the currency of your choice instead of USD. 

  
# What happens behind the scenes?

Upon checkout using your SaaS link, a customer profile is created in your Stripe account, along with an associated subscription, payment, and invoice (if no trial is offered)

![](https://s3.amazonaws.com/cdn.freshdesk.com/data/helpdesk/attachments/production/155010057041/original/tPOVWtT5ig-dG6qGvrO0fjqx4HTCXHiFmA.png?1697198368)

![](https://s3.amazonaws.com/cdn.freshdesk.com/data/helpdesk/attachments/production/155009975828/original/_zNLJXZUseVxZHCZ5CVX6JvfGPFbPS4V0Q.png?1697124190)

  
The [invoice](https://storage.googleapis.com/ghl-test/whcJGypGlr1gJ9kdfvIC/media/6528106941c4a93d52bff4a4.pdf) and [receipt](https://storage.googleapis.com/ghl-test/whcJGypGlr1gJ9kdfvIC/media/6528106941c4a95131bff4a3.pdf) will also be in your currency instead of USD.

  
# But I want to use my funnel to sell this instead of Checkout links. How can I do that?

If you wish to use HighLevel funnels to sell your SaaS products instead of using the checkout link, then you can simply import these prices (the once we updated to your currency instead of USD) to that sub-account as shown below.

  
Make sure the Stripe account connected to your sub-account (location) that you'd use to sell your SaaS products is the same as the Stripe account connected to your agency.
  
  
You can check the Stripe account connected to a sub-account (location) by visiting Location Level -> left menu -> payments -> integrations

  
![](https://s3.amazonaws.com/cdn.freshdesk.com/data/helpdesk/attachments/production/155009977185/original/urZ5-b3HRWwEOkxLcmjtWvHqA0igt4HA0Q.png?1697124967)

  
You can check the Stripe account connected to the agency by visiting Agency Level -> left menu -> Settings -> Stripe

  
![](https://s3.amazonaws.com/cdn.freshdesk.com/data/helpdesk/attachments/production/155009977428/original/EE4E1t2oyUeZlpmctMlyEQQAZNPlV1YgRw.png?1697125047)

  
Once you have validated that both Strip accounts are the same you can start importing your SaaS products in that sub-account (location).

  
## How can I import my modified SaaS products and prices to the sub-account (location) I want to use for selling SaaS?

  
Head over to Location Level -> left menu -> payments -> products and click on "Import from Stripe" button. Then search for your SaaS product and click import.

  
![](https://s3.amazonaws.com/cdn.freshdesk.com/data/helpdesk/attachments/production/155009978053/original/27vKd3PO_-Oi6lD16lzoMLk2xWHy70wSqg.png?1697125244)

![](https://s3.amazonaws.com/cdn.freshdesk.com/data/helpdesk/attachments/production/155009978972/original/3MWNCYx8mLNZCqi92xlhb43KPMS6kAzbXg.png?1697125550)

  
Repeat this for all your SaaS products & prices. Your screen should look like this.

  
![](https://s3.amazonaws.com/cdn.freshdesk.com/data/helpdesk/attachments/production/155009985010/original/eWUIR90lbwwsJjclWuCirEcwva2NxcawxQ.png?1697128332)

![](https://s3.amazonaws.com/cdn.freshdesk.com/data/helpdesk/attachments/production/155009985058/original/6eddlGzEbt2-7wJM9mRobbVLsa96_oi48A.png?1697128373)

  
As you may notice all imported prices are in the currency of your choice instead of USD. 

  
Now you can simply [add these products to your funnel's one step or 2-step order forms](https://help.gohighlevel.com/support/solutions/articles/48001184920-saas-mode-full-setup-guide-faq#Setting-up-your-Funnel/-Website) and start selling!

  
# What about the wallet recharges (credits)?

Yes, the sub-account credit charges (wallet recharges) will also be in the currency of your choice. However please keep in mind the usage will still be shown in USD.

  
The charge to your customers (invoices & receipts) will be in your currency.

However, in the usage records (inside HighLevel -> Location level -> left menu -> settings -> company billing) usage will still show up in USD. 

  
For example in this case, the user added US$ 100 to their credits. It shows up like this in their usage records

  
![](https://s3.amazonaws.com/cdn.freshdesk.com/data/helpdesk/attachments/production/155009985968/original/dcSLSa5AlEy5fh3lLnOJU9TM4FlLA5Zw2A.png?1697128784)

  
Behind the scenes, HighLevel automatically converts this amount (US$ 100) to your currency (AUD in this example) and runs the charge on Stripe in your currency. Thats why you would see the associated receipt to be in the currency of your choice. 

  
![](https://s3.amazonaws.com/cdn.freshdesk.com/data/helpdesk/attachments/production/155009986380/original/BHEccV8xipyuF-GbKRzjxcvT2QjjBB9QIw.png?1697128932)

  
Please look at [this receipt](https://pay.stripe.com/receipts/payment/CAcaFwoVYWNjdF8xSUVEekxCeVZsZklUdlJYKJbDoKkGMgaVsKjTnBM6LBaPStnFOeAWtrXYuHCf1Nx0hjxv%5Fs62yJtVUxM6b7qMCvZK-HMJV6xnsfbn) for reference. 
  
  