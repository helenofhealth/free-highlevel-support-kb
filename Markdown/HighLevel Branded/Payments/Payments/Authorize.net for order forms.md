**Date Updated:** 2023-11-14T14:42:46.000Z

Authorize.Net is considered a competitive payment processor due to its reliability, security, and wide range of features. It has operated for over 20 years, providing payment processing services to businesses of all sizes. Authorize.Net provides robust security measures to protect transactions, sensitive customer information, and reliable uptime to ensure smooth transactions. Additionally, Authorize.Net offers features such as recurring billing, mobile compatibility, and integrations with popular e-commerce platforms.,
  
  
#### **Covered in this Article**

#### [**Which Payment Processor to use?**](#Which-Payment-Processor-to-use?)

#### **[Requirements to use Authorize.Net](#Requirements-to-use-Authorize.Net)**

#### **[How to integrate Authorize.Net as a Payment Gateway?](#How-to-integrate-Authorize.Net-as-a-Payment-Gateway?)**

#### **[Side Notes for using Authorize.Net](#Side-Notes-for-using-Authorize.Net)**

#### **[Test cards for Authorize.net integration. ](#Test-cards-for-Authorize.net-integration.%C2%A0)**

####   
[**FAQ**](#FAQ)

#### [Why don't I see Paypal among the default gateway options?](#Why-don't-I-see-Paypal-among-the-default-gateway-options?)

#### [What will change in the reporting of transactions done with Authorize.net? Where will I be able to keep track of all payments?](#What-will-change-in-the-reporting-of-transactions-done-with-Authorize.net?-Where-will-I-be-able-to-keep-track-of-all-payments?)

#### [Where will I be able to find the subscriptions created via Authorize.net? I cannot relate to the subscription status defined on the Subscriptions page.](#Where-will-I-be-able-to-find-the-subscriptions-created-via-Authorize.net?-I-cannot-relate-to-the-subscription-status-defined-on-the-Subscriptions-page.)

#### [How do I Cancel/End a subscription created via Authorize.net? I am not able to do so in the merchant portal.](#How-do-I-Cancel/End-a-subscription-created-via-Authorize.net?-I-am-not-able-to-do-so-in-the-merchant-portal.)

#### [Will I be able to refund transactions as well within the application itself?](#Will-I-be-able-to-refund-transactions-as-well-within-the-application-itself?)

#### [I am using FDS filters with Authorize.net to hold transactions for review if the address is not submitted, the card code is not submitted, etc. Is the system compatible with handling those cases?](#I-am-using-FDS-filters-with-Authorize.net-to-hold-transactions-for-review-if-the-address-is-not-submitted-or-the-card-code-is-not-submitted-etc.-Is-the-system-compatible-with-handling-those-cases?)

#### [When will Authorize.net be available for invoices/Text2Pay/Calendar payments/memberships and other areas?](#When-will-Authorize.net-be-available-for-invoices/Text2Pay/Calendar-payments/memberships-and-other-areas?)
  
  
---

## **Which Payment Processor to use?**

Deciding between Stripe, PayPal, and Authorize.net will depend on what's best for your business. Here's a comparison:

  
**Stripe:** A popular choice for online businesses and startups, Stripe offers a developer-friendly platform, custom integrations, and transparent pricing.

  
**PayPal:** PayPal is a well-established payment processor with a global presence and a wide range of features, including a secure payment gateway, invoicing, and recurring payments.

  
**Authorize.net:** Authorize.net is a trusted payment processor with a long history of providing reliable and secure payment processing services. It offers comprehensive features, including fraud detection and mobile compatibility.

  
Ultimately, the best choice depends on the specific needs of your business, such as the types of payments you need to accept, your target market, and your budget. It's recommended to compare each processor's features, fees, and support options before deciding.

  
![](https://s3.amazonaws.com/cdn.freshdesk.com/data/helpdesk/attachments/production/48278589425/original/uuTirde8-8iEPL9WDkQhaAoDGMfz7n97AA.png?1675099374)

**Please Note:**

The data for fees is accurate as of when this article is being published, for more information please check out the Pricing pages of the three options listed:  
  
**Stripe: <https://stripe.com/gb/pricing>**  
**Paypal: <https://www.paypal.com/us/webapps/mpp/merchant-fees>**  
**Authorize.net: <https://www.authorize.net/en-us/sign-up/pricing.html>**

  
---

## **Requirements to use [](//Authorize.net)Authorize.Net**

  
Authorize.net can accept transactions from [United States, Australian, and Canadian](https://support.authorize.net/knowledgebase/Knowledgearticle/?code=000001207) merchants.  
Currencies supported with [Authorize.net](http://Authorize.net) \- [Link](https://support.authorize.net/knowledgebase/Knowledgearticle/?code=000001207)

  
Before you can integrate [Authorize.Net, ](//Authorize.Net) you must confirm whether you are on a browser that supports using it.

  
**Below is a list of supported and tested browsers:**

  
| **Browser Name** | **Recommend Version** |
| ---------------- | --------------------- |
| Chrome           | v80 or higher         |
| Edge (Chromium)  | v85 or higher         |
| Firefox          | v78 or higher         |
| Safari           | v12 or higher         |

  
You can check and verify the browser and version you are using by:

  
Use the below help/about information when inside the respective browser:  
**[Chrome](https://www.google.com/chrome/update/)**

**[Edge](https://support.microsoft.com/en-us/microsoft-edge/find-out-which-version-of-microsoft-edge-you-have-c726bee8-c42e-e472-e954-4cf5123497eb)**

**[Firefox](https://support.mozilla.org/en-US/kb/find-what-version-firefox-you-are-using)**

**[Safari](https://support.apple.com/safari)**

  
Utilize sites like:

<https://www.whatsmybrowser.org/>

<https://www.whatismybrowser.com/>

  
For the Merchant Interface inside Authorize.net, if an unsupported browser or version is detected, two possible messages may display depending on how low the browser version is.,

  
**Browser Warning/Out of Date** – In this case, Authorize.net may have detected a browser/version that you may encounter issues with. You should update to a newer version or use a different supported browser. 

  
**Examples of Outdated browsers:**

  
Internet Explorer (IE) 11

Edge (Legacy)

Opera

  
![](https://s3.amazonaws.com/cdn.freshdesk.com/data/helpdesk/attachments/production/48278762635/original/GKfxv8yq-4fvH8Z_imbBLYO_QymhEZHU3Q.png?1675167685)

  
**Browser Block/Out of Date** – In this case, we have detected a browser/version that will encounter issues, and an updated browser version needs to be used or a different supported browser.

  
![](https://s3.amazonaws.com/cdn.freshdesk.com/data/helpdesk/attachments/production/48278762749/original/KtjM7pJ7sGxe3bSPyQzvG-RIDVMfNuDZhQ.png?1675167724)

---

  
## **How to integrate [](//Authorize.net)Authorize.Net as a Payment Gateway?**

1\. Once you are sure you are using a supported browser and that you are operating from within one of the supported countries, [you will need to acquire Live and Sandbox API keys from Authorize.net](https://developer.authorize.net/hello%5Fworld/common%5Fsetup%5Fquestions.html#:~:text=How%20do%20I%20obtain%20the%20transaction%20key%20for%20my%20sandbox%20account%3F)

  
For sandbox API keys, log into the [sandbox Merchant Interface](https://sandbox.authorize.net). For Live API keys, log into the [Live Merchant Interface](https://account.authorize.net).

  
[Click Here](https://developer.authorize.net/hello%5Fworld/testing%5Fguide.html) for more details on Sandbox vs. Live Mode in [Authorize.Net](//Authorize.net).

---

---

2\. Then you can proceed to **Payments> Integrations>**Drop the 3 API Keys you got from your **Merchant Interface** in [Authorize.Net](//Authorize.net). 

  
You can input the **Live API Keys** in the Live fields.

![](https://s3.amazonaws.com/cdn.freshdesk.com/data/helpdesk/attachments/production/48278804144/original/HOBNH3in9ASQb-G6x7kYxlwqQhUtTsHISw.png?1675175721)

  
And you can input the **Sandbox API Keys** in the Sandbox Fields.

![](https://s3.amazonaws.com/cdn.freshdesk.com/data/helpdesk/attachments/production/48278804449/original/c1PlVkmiNqkN6Ajbwb52IMMBB-Q1Lz-4yQ.png?1675175803)  

Once inputting the desired API Keys, click on the **Save** Button.  
  
![](https://s3.amazonaws.com/cdn.freshdesk.com/data/helpdesk/attachments/production/48278806039/original/ab0_IqVbPs2X9Vub6cIQlq3doNO09HHYBQ.png?1675176076)

  
3\. It will show you a quick prompt asking whether you want to make [](//Authorize.net)Authorize.Net[ ](//Authorize.net) your Default Payment Gateway.  
  
![](https://s3.amazonaws.com/cdn.freshdesk.com/data/helpdesk/attachments/production/48278806389/original/IL6l8BahVDEvcCMpvO9j4AqAB8Uqh_Y17A.png?1675176142)

Clicking on **Cancel** will still integrate [](//Authorize.net)Authorize.Net but will not make it the Default Gateway.

  
![](https://s3.amazonaws.com/cdn.freshdesk.com/data/helpdesk/attachments/production/48278806859/original/77rhBaAuwHnXc3dSD99tCHCV_zJ6ygbNZA.png?1675176231)

  
Clicking on **Confirm** will integrate [](//Authorize.net)Authorize.net[](//Authorize.net) and make it the Default Payment Gateway.

![](https://s3.amazonaws.com/cdn.freshdesk.com/data/helpdesk/attachments/production/48278807334/original/ehWEyfGMBx06EEmV6-kny_h2Mbvr-ds-zw.png?1675176320)

  
**Please Note**

You are not required to disconnect **Stripe** to connect to **Authorize.net**. You can connect to both gateways on the integrations page. However, since you have connected two different gateways for processing payments, you will need to define a default gateway for processing payments. **PayPal** will continue to function alongside Authorize.net/Stripe in order forms, whichever is set as the default 

  
---

## **Side Notes for using Authorize.Net**

If Authorize.net is connected and set as the default gateway, other product areas like memberships and SAAS payment links will continue to process payments using Stripe. 

If there are recurring subscriptions/pending transactions with Stripe, they will continue to run as is until the Stripe connection is in place. We encourage you not to disconnect any gateway. Defining the default gateway will run new transactions through the desired choice and keep the existing subscriptions running through Stripe and PayPal integrations in place.

  
**Please Note:**

  
You need to [upgrade to funnels version 2](https://help.gohighlevel.com/support/solutions/articles/48001204903-how-to-upgrade-a-version-1-funnel-to-version-2-) to make use of this feature.

  
[Click here](https://account.authorize.net/help/Miscellaneous/FAQ/Frequently%5FAsked%5FQuestions.htm) for the link to [](//Authorize.Net)Authorize.Net[](//Authorize.Net)'s FAQ section.

  
### **Test cards for Authorize.net integration.** 

Expiry Date can be any future date, and any 3/4 digits value can be the CVC: 

  
4007000000027 (Visa)

4012888818888 (Visa)

4111111111111111 (Visa)

370000000000002 (American Express)

5424000000000015 (Mastercard)

2223000010309703 (Mastercard)

2223000010309711 (Mastercard)

6011000000000012 (Discover)

3088000000000017 (JCB)

38000000000006 (Diners Club/ Carte Blanche)

---

## **FAQ**

### **Why don't I see Paypal among the default gateway options?**

You can connect to Paypal and use it as a payment method alongside a credit card payment method using Stripe/Authorize.net. This means the default has to be chosen among Stripe/Authorize.net when connected. PayPal can be used independently and alongside credit card payment methods on order forms. and 

  
### **What will change in the reporting of transactions done with Authorize.net? Where will I be able to keep track of all payments?**

There will be no change in the Orders/Subscriptions/Transactions reporting. All the payments done via Authorize.net will be available under Payments ➝ Transactions. 

  
![](https://s3.amazonaws.com/cdn.freshdesk.com/data/helpdesk/attachments/production/48278810849/original/6FPZdXeiv4MDSp1d36218_ezuIA6CZaUEA.png?1675177050)

  
Also, there will be no change in the functioning of workflow triggers/attribution associated. All the functionalities will work the same with Authorize.net.

###   

### **Where will I be able to find the subscriptions created via Authorize.net? I cannot relate to the subscription status defined on the Subscriptions page.**

  
All subscriptions created on the order forms can be tracked under **Payments ➝ Subscriptions**. 

![](https://s3.amazonaws.com/cdn.freshdesk.com/data/helpdesk/attachments/production/48278816562/original/SP8Q-LT4WctAzVMUVMK7OvsFSnxFFOdYXQ.png?1675178073)

The following list represents subscription statuses and their inferences: 

  
**Pending** \- When held for merchant review due to FDS

**Trial** \- Subscription is in trial mode

**Active** \- Last payment was made, and there is an upcoming payment as well

**Expired** \- All the subscription payments have been completed, and the subscription no longer exists

**Canceled** \- The merchant canceled the subscription using the Cancel action, and no further payments are to be processed.

**Unpaid** \- The last payment for the subscription was not paid successfully. The subscription is ongoing, but the final payment was unsuccessful.
  
  
Cancellation will be possible for the subscriptions according to the status: 

  
| **Status** | **Cancel** |
| ---------- | ---------- |
| Pending    | No         |
| Trial      | Yes        |
| Active     | Yes        |
| Expired    | No         |
| Canceled   | No         |
| Unpaid     | Yes        |
  
  
Cancel Action is provided only against those subscriptions which are created on Authorize.net. Cancellation of subscriptions for Stripe and PayPal will be added soon. 

  
**The following flow describes the handling of subscription statuses and payment retry logics in case of a subsequent payment failure :**

  
* If the first subscription payment is successful while purchasing the subscription on the order form, the subscription will move into the active state  
   * It can also move into the trial status if there is a trial period attached to the recurring product
* The subscription will remain active until every recurring payment is made successfully for the subscription and will move to "Expired" after the completion of payments.
* If the credit card expires for the end customer in the middle of the subscription, the payment requires authentication from the end customer, or the last payment didn't go through successfully; the status will move over to "Unpaid."  
   * The payment will be attempted two more times after 24 hrs each. The status will remain "Unpaid."  
   * The subscription will remain in the Unpaid state and will attempt the following subsequent transactions, each with two retries.  
   * The next subsequent payment will also be attempted, and if any payment becomes successful, the subscription will move into "Active." Else will stay with "Unpaid" status.  
   * The subscription status will move to "Expired" after all the retries have been made for the last transaction.
* If the merchant disconnected the gateway account and there is an ongoing subscription, the transaction cannot be processed; hence the subscription will move to unpaid. The retry attempts will continue according to the retry logic.

  
### **How do I Cancel/End a subscription created via Authorize.net? I am not able to do so in the merchant portal.**

Subscriptions created using Authorize.net can be canceled within the **Subscriptions** page using the  
'**Cancel Subscription**' Action.

![](https://s3.amazonaws.com/cdn.freshdesk.com/data/helpdesk/attachments/production/48278812831/original/oNCJoq-nbfZtbm7bWPTcq0W76vqY2OQ_dA.png?1675177378)

![](https://s3.amazonaws.com/cdn.freshdesk.com/data/helpdesk/attachments/production/48278814793/original/SzIQaM8S3zpPx-44Zl2HltXRq_KMN3pTow.png?1675177713)

  
We do not create subscriptions using the Automatic Recurring Billing of Authorize.net; hence, only transaction charges corresponding to a subscription will be visible in the merchant portal. 

  
### **Will I be able to refund transactions as well within the application itself?**

No, we do not have the refund functionality within the application. It would be best if you used the merchant portal for refunding transactions.

  
### **I am using FDS filters with Authorize.net to hold transactions for review if the address is not submitted, the card code is not submitted, etc. Is the system compatible with handling those cases?**

Yes, If you hold transactions submitted on order forms for review based on FDS filters. In that case, your transaction will be held for review (or declined as per the setting that you have configured) and will be visible in your merchant portal. Additionally, the corresponding status will be updated on the Transactions page. When you approve or decline the transaction.

  
Regarding recurring invoice payments/calendar appointment booking payments, we treat the transaction as declined and do not book the calendar appointment or schedule the auto payment, since it introduces complications regarding when the business owner will approve the payment.

  
### **Does Authorize.net work for membership checkouts?**

Yes, [Authorize.net](//Authorize.net) is available for membership checkouts

  
### **When will Authorize.net be available for SaaS?**

Please vote on the ideas board for enabling this integration for selling SaaSallowing this integration.