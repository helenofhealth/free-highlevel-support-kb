**Date Updated:** 2023-12-15T20:44:47.000Z

  
---

**TABLE OF CONTENTS**

* [Introduction](#Introduction)  
   * [What are Webhooks?](#What-are-Webhooks?)  
   * [How do Webhooks Work?](#How-do-Webhooks-Work?)
* [How to Use Webhooks in HighLevel](#How-to-Use-Webhooks-in-HighLevel)  
   * [(A) Inbound Webhook ](#%28A%29-Inbound-Webhook%C2%A0)  
   * [(B) Outbound Webhook](#%28B%29-Outbound-Webhook)
* [FAQs](#FAQs)  
   * [What is Zapier, Make, or Pabbly?](#What-is-Zapier,-Make,-or-Pabbly?)  
   * [Getting Started with Zapier](#Gettings-Started-with-Zapier)  
   * [What are the Differences Between API and Webhooks?](#What-are-the-Differences-Between-API-and-Webhooks?)

---

  
# Introduction

Needing some information from another application you use? Webhooks are certainly one of the first choices for many users, as they greatly increase your ability to send information from one place to another. If our powerful HighLevel Workflow Automations are not able to perform a task for you - chances are that a webhook can... Or at least get you close!

  
In this article, we will walk through how to use webhooks in HighLevel. 

  
## What are Webhooks?

HTTPS request (or webhooks) powers nearly everything you interact with on the internet. Webhooks are what allow applications like HighLevel to talk to Stripe, Twilio, Mailgun, Zapier, and more. Now, you can have full access to webhooks to make your business needs come alive!

  
Webhooks are a great way to connect applications. Webhooks allow platforms to communicate to complete unique tasks by connecting applications together. Below we will review common terms when using Webhooks.

  
**Helpful Def** **initions:**

* HTTPS Request \- The official term for the type of request a webhook is… An HTTP is the primary way to send information between websites and web browsers. HTTPS is a more secure version, which encrypts the data when it is transferred.
* Triggering Event \- The unique event that occurs, signaling an app to send information to the Webhook URL of another app.
* Webhook URL \- A unique URL created by the app receiving a webhook request. It’s kind of like an address or phone number.
* Payload \- refers to all of the information packaged and sent from one app to another.
* Query Params \- much like UTM Parameters, Query Params are a helpful way to map information using the Webhook URL. Which can be better used by the receiving application when mapping the payload.
* Mapping \- Like connecting the dots, mapping is the process of taking the payload received and “mapping” to the correct fields for use in the receiving application. For example, the payload has a contact name, email, and purchased service name. You will need to “map” or connect this information from the payload, into the correct custom fields for the contact within the HighLevel Workflow.

  
## How do Webhooks Work?

Generally, webhooks are used to connect applications. They require a triggering event that signals one app to send the request to another app. For example, a purchase happens in your payment software Stripe, which will be sent to HighLevel. So Stripe will package the information up into a “payload” (or the information sent out) which is sent to HighLevel. In HighLevel, the information received can then be used to perform tasks.

  
To use Webhooks, one application needs to provide the Webhook URL. A Webhook URL is a unique URL created by the app receiving a webhook request. It’s kind of like an address or phone number. When you want to call a business, you require their unique phone number and even an extension at times to get to the right department. A Webhook URL is much the same - it is a unique phone number used to make a call request to.

  
**Use Case Example**

You own a Shopify eCommerce store that utilizes Stripe to process your payments. You want to use HighLevel to send emails to specific users who have purchased a specific course. However, the information from the purchases is not in HighLevel - so you don't know who purchased what. To send emails to the correct contacts in HighLevel, you will need to create a webhook event to fire into HighLevel every time that specific product is purchased in Stripe. HighLevel can then use this information to perform specific tasks, like sending emails to those specific contacts who purchased the product.

  
![](https://s3.amazonaws.com/cdn.freshdesk.com/data/helpdesk/attachments/production/155010241068/original/e_ZtUPbrIo3urqJR16g_RzagAV2I0i0UIQ.png?1697473846)

  
In this scenario, you will use the HighLevel Workflow trigger "inbound Webhook" to catch the information from Stripe. To make it easier, we recommend you use Zapier or another automation software, to trigger when the purchase is made in Stripe (if you are not using a HighLevel Order Form or Product). When the purchase is made, a payload is packaged up with all of the information you need in HighLevel. HighLevel catches and receives the information that is used to perform your specific tasks. In this case, marketing to your buyers who bought that specific product.

  
That's the overview of webhooks, but there is A LOT more to learn. For now, this will get you started. Below, we will review the two ways you can use webhooks in HighLevel.
  
  
---

# **How to Use Webhooks in HighLevel**

There are two ways to utilize Webhooks in HighLevel. In potentially over-simplistic terms, there are “Catching” and “Sending” Webhooks.

  
**Two ways to use Webhooks in HighLevel:**

(A) Inbound Webhook

“Catching” an Inbound Webhook Request in a HighLevel Workflow Trigger.

As the names suggest “Catching” is all about receiving or “catching” a webhook request made to the HighLevel Webhook URL. In HighLevel, this is a Workflow Trigger called an “Inbound Webhook.”

(B) Outbound Webhook

 “Sending” an Outbound Webhook Request with a HighLevel Workflow Action.

In contrast to the above “Catching” motion… “Sending” is when you make a request to an external Webhook URL. In HighLevel, this is a Workflow Action called “Webhook.”

  
Below, we will walk through each scenario and how to perform it in HighLevel.

  
**Order: Trigger, Action, Trigger, Action**

Another helpful way to learn about webhooks is to see the pattern in the order of operations that occur. Regardless of an inbound or outbound webhook we generally have a Trigger and action in one app that then sends information to another app. In this second app, there is another trigger and then the last action. 

  
Hence the title... Order: "trigger, action, trigger, action." Which denotes the flow of webhooks that are utilized by both apps. Each has a single trigger and action that causes a connection between the two.

  
You will notice this same pattern in the examples below with the first app having a trigger and action --> which sends a payload to the next app that is an inbound webhook trigger followed by another action.

  
![](https://s3.amazonaws.com/cdn.freshdesk.com/data/helpdesk/attachments/production/155012254101/original/YacUVsLrhrnYCOA1oPdfbOmoKMSGRJrKsg.png?1699461803)

---
  
  
## **(A) Inbound Webhook** 

**“Catching” an Inbound Webhook Request in a HighLevel Workflow Trigger.**

  
In this scenario, we want HighLevel to catch information from an external app. The external app will send the Payload to the HighLevel Webhook URL provided when we create a Workflow Trigger - Inbound Webhook. For example, our use case above is an inbound webhook request where we send information from an external purchase into HighLevel to be used to perform unique tasks for those specific contacts who purchased the product.

![](https://s3.amazonaws.com/cdn.freshdesk.com/data/helpdesk/attachments/production/155012254156/original/6YZqHiH1BZQqlkiyYujW_cqCd1Gvz3881Q.jpg?1699461860)

  
**1\. Enable Inbound Webhooks**

If you haven’t already, you will need to [enable “LC Premium Triggers & Actions” ](https://help.gohighlevel.com/en/support/solutions/articles/48001231559)in order to proceed. To catch an inbound request, we need an “Inbound Webhook” which is only available on LC Premium Triggers & Actions.

  
**Did you know...** Most HighLevelers like to utilize integration and automation software like Zapier, Make, or Pabbly. They come with easier-to-use triggers and actions for many applications you may be using already. In many cases, it is simpler and more powerful to utilize one of these platforms in combination with HighLevel Workflows. [Learn more about Zapier, Make, and Pabbly here](https://help.gohighlevel.com/a/solutions/articles/155000001183/edit?portalId=48000045315#What-are-the-Differences-Between-API-and-Webhooks?).
  
  
**2\. Create the Webhook URL in a HighLevel Workflow Trigger**

Now we need to open our HighLevel Workflow and create the Webhook URL. Open/Create your workflow then select the “Inbound Webhooks” as the Workflow trigger. A HighLevel Webhook URL will be created. Copy this Webhook URL to be used in the next step.

![](https://s3.amazonaws.com/cdn.freshdesk.com/data/helpdesk/attachments/production/155010241062/original/zZZV8sXYGtNPfk_DIGZQc4wmzSezGmKfEA.png?1697473842)
  
  
**3\. In the External App, Create a Webhook Action Step**

In your external app of choice, you will need to create a trigger and webhook action step. For example: In Zapier, you can use a “Payment” trigger to fire when a payment is made. We can use the “Webhooks By Zapier” to POST the payload to the HighLevel Webhook URL. Paste the HighLevel Webhook URL from step two into the Zapier Action Step.

  
![](https://s3.amazonaws.com/cdn.freshdesk.com/data/helpdesk/attachments/production/155011887200/original/IKDL_daUhGv_gqbybrdd9RALZoIuj56fsw.png?1699043799)
  
  
**4\. Send a Test**

Now we need to send a sample payload to our HighLevel Webhook URL in order to proceed. Within your external app, Zapier in this example, go to the end of the step and hit “Test Step.” For sending a test payload in HighLevel for an external app, please consult your external app documentation and Support. In HighLevel, continue to wait and refresh the “Mapping Reference” Section until you have a “Mapping Reference” in HighLevel available to select.

  
![](https://s3.amazonaws.com/cdn.freshdesk.com/data/helpdesk/attachments/production/155011887243/original/M5bHGIPHDZ8foG5ik_NZlUF86q6Lk4QbxA.png?1699043936)

![](https://s3.amazonaws.com/cdn.freshdesk.com/data/helpdesk/attachments/production/155010241070/original/IOAjncnP7_DzLx_BrkksQdSwP2Hv43Ncdg.png?1697473846)

![](https://s3.amazonaws.com/cdn.freshdesk.com/data/helpdesk/attachments/production/155010241069/original/QoSSEVtaJAx113nCW8stk0LNM4J8Vv4rhQ.png?1697473846)
  
  
**5\. Create/Update Contact**

For HighLevel, we require a contact for every single Automation to run. This is why the “Create/Update Contact” will open automatically. You can also use the "Find Contact" Action to locate a contact based on a custom field or another value. It is required to have this filled out, otherwise, this will NOT work and the Workflow will break. So at minimum, create/update the phone or email from the payload of the inbound webhook or find a contact based on a custom field or such. A contact found or matched is required in order for this to work.

  
![](https://s3.amazonaws.com/cdn.freshdesk.com/data/helpdesk/attachments/production/155010241065/original/1jIFtXcVBneM-vnEM2w50nn0Zx8VQW_AvQ.png?1697473844)

  
Now you are done! You have the information in HighLevel to map and use as you like within the Workflow.

  
**Mapping Information in HighLevel**

Now you can use this information within "Custom Values" > "Inbound Webhook Trigger" to map the information from the payload into the correct fields or actions in HighLevel. So when it runs, the right information from the Inbound WEbhook will populate in the correct place in HighLevel.

  
![](https://s3.amazonaws.com/cdn.freshdesk.com/data/helpdesk/attachments/production/155010246863/original/vQ-E_DHbKtdc6AQblQyV1MWKzmRaAr-JMQ.png?1697478103)

  
Learn more about [Inbound Webhooks in HighLevel here](https://help.gohighlevel.com/en/support/solutions/articles/48001237383).

  
Want to learn more about Zapier and how to use it?[ Getting Started with Zapier](#Gettings-Started-with-Zapier).

  
---
  
  
## **(B) Outbound Webhook**

**“Sending” an Outbound Webhook Request with a HighLevel Workflow Action.**

  
In this scenario, we are sending information from a HighLevel Workflow Action into an external app. For example, when someone fills out a form in HighLevel, we want this contact information to go into an External App so we can have the information about the contact there. 

  
![](https://s3.amazonaws.com/cdn.freshdesk.com/data/helpdesk/attachments/production/155012254224/original/5q0UMpKWjfR7oeR83CDvnC5F3u5DsL-H-w.jpg?1699461932)
  
  
**1\. Ensure that the External application allows for Receiving of Webhook Data**

For some external applications, receiving data from a webhook is a premium Feature. Other apps just simply need to have the trigger enabled. You will need to consult the documentation for the application and upgrade if needed. In Zapier, which we will use in this example, you must be on a paid account to use inbound Webhooks (known as Catchhooks) by Zapier.

  
**Not Seeing Webhooks in Your External App?**

In some cases, webhooks may not be available within many External Apps for you to use. In these cases, you can check out automation/integration software like Zapier, Pabbly, or Make to bridge the information gap between your apps. [Learn more about Zapier, Make, and Pabbly here.](https://help.gohighlevel.com/a/solutions/articles/155000001183/edit?portalId=48000045315#What-is-Zapier,-Make,-or-Pabbly?)
  
  
**2\. Create a Webhook URL in the External App**

Within your External App create a trigger for the Inbound Webhook. After creating this Trigger, you should have a Webhook URL generated to be used in later steps. For example: In Zapier, you can use the “Webhooks By Zapier” Trigger with the “Catch Hook” Event. Continue to the Trigger step. Copy the Webhook URL generated from the External App.

![](https://s3.amazonaws.com/cdn.freshdesk.com/data/helpdesk/attachments/production/155011887769/original/99_GnzVBey8hlc2BEYFqP1rDczbd1xANaA.png?1699044740)
  
  
**3\. Add the External Webhook URL to your HighLevel Workflow Action**

Now we can add the External Webhook URL to a HighLevel Workflow Action. Create or open your HighLevel Workflow. Add the External Webhook URL to a HighLevel Workflow Action. Save the workflow and publish it.

![](https://s3.amazonaws.com/cdn.freshdesk.com/data/helpdesk/attachments/production/155011887762/original/fujjPdM8233Nf86d5zUGqqtfw0wMTZVm7Q.png?1699044726)
  
  
**4\. Send a Test From HighLevel to the External App**

Now we need some sample information from HighLevel to the External App. To do this, we need to trigger the workflow. For example, we can make a Test purchase so the Workflow Trigger will fire this information to Zapier. It is best to perform the workflow trigger as if it is a live-action of what will happen. This is because you want all of the example data provided in the payload when you go to use it in the External App.

  
Continue testing until you have successfully sent the information to the External app and it has been received by the External App.

  
![](https://s3.amazonaws.com/cdn.freshdesk.com/data/helpdesk/attachments/production/155010241075/original/UsPpaTNGd2xqxNTsUwcV6GEjTbE53oEzuQ.png?1697473846)

  
Well done! Now every time the HighLevel Workflow triggers, it will send this information to your External App for usage. Within Zapier, you can now use this information to populate Spreadsheets or perform other unique tasks.

  
**Mapping Information in Zapier**

Select a field to update on your Zapier action, and then a popup will show an "Insert Data" which will allow you to select a placeholder (or Custom Value as it is known in highLevel) within the Zapier action to map the information in the payload. This will stamp the data you want during every run of this webhook so the correct inforamtion from HighLevel updates the correct places in Zapier or your other third party app. 

  
![](https://s3.amazonaws.com/cdn.freshdesk.com/data/helpdesk/attachments/production/155012266200/original/ap9P2cWxw5xgAWgbxJ8ydYNicpe8ARTbpg.png?1699474788)

  
Want to learn more about Zapier and how to use it?[ Getting Started with Zapier](#Gettings-Started-with-Zapier).

  
---

# FAQs

  
## What is Zapier, Make, or Pabbly?

Zapier, Make or Pabbly are all Automation and integration software. Meaning they exist to help connect applications together. They do this with pre-built connections to apps you can integrate into them. After integrating, you can use a number of triggers and actions - much like you can in HighLevel Workflows. However, these are triggers and actions for other applications. 

  
For example, did you know we have integrations with these softwares? Visit the links below from the most common platforms we have seen HighLevelers use.

  
[Zapier LC Integration](https://zapier.com/apps/leadconnector/integrations)

[Make LC Integration](https://www.make.com/en/help/app/highlevel-leadconnector)

[Pabbly LC Integration](https://www.pabbly.com/connect/integrations/highlevel/)

  
What makes these more powerful is combining these pre-built triggers and actions with webhook actions. This will open an entire world of possibilities. You certainly can’t do everything… But hey… It’s better than coding a custom integration from scratch using an API. At least they are pre-built and with webhooks, most of your tasks can be fully (or partially) automated.

  
## Getting Started with Zapier

Zapier is one of the most commonly used Automation and Integration Software. With thousands of pre-built triggers and actions between apps or platforms, it is a handy tool. If you are getting started with Zapier and not sure how to use it, check out their quick and informative Courses.

  
<https://zapier.com/resources/guides/quick-start/automation-basics> 

<https://learn.zapier.com/intro-to-automation> 

<https://learn.zapier.com/path/a-complete-guide-to-lead-management>

  
Check out these links above to get started with Zapier today!

  
## What are Query Params?

Query Params are a great way to pass in information via a webhook. It is much like UTM parameters, in that they add information to be used by the receiving application. For example, ClickUp is a popular task management app. When you send information from ClickUp into HighLevel, the custom field does not come in cleanly. Which is a bummer, custom fields are a critical part of the information we need. So we can pass in the information we need more cleanly with Query Params.

  
All you have to do is add a query key and then the custom value to the Webhook URL. For example, our webhook URL is "https://services.leadconnectorhq.com/hooks/pgWooooooooG57D/webhook-trigger/ce000-800f-4bec-0090-f000000000" so then we can add a query key and a value to the URL like "[https://services.leadconnectorhq.com/hooks/pgWooooooooG57D/webhook-trigger/ce000-800f-4bec-0090-f000000000](https://services.leadconnectorhq.com/hooks/pgWooooooooG57D/webhook-trigger/ce000-800f-4bec-0090-f000000000?custom%5Ffield={{click.up.custom.field)[?custom\_field={{click.up.custom.field](https://services.leadconnectorhq.com/hooks/pgWooooooooG57D/webhook-trigger/ce000-800f-4bec-0090-f000000000?custom%5Ffield={{click.up.custom.field).value}}"

  
![](https://s3.amazonaws.com/cdn.freshdesk.com/data/helpdesk/attachments/production/155011888492/original/irJ6Vrg9RhGYNfIVxSzMwGcNKIOJGGFaKg.png?1699046037)

  
After sending this to HighLevel, you are then able to select the query parameter cleanly. You can add as many as you like.

  
## What are the Differences Between API and Webhooks?

Application Programming Interface (API) is the back end (or back door) connection between apps. If you can’t do it natively within the app, chances are, you can find some API Documentation to help you achieve it or get close to it. The only issue is… API is complex to use, hence the wording “language.” It is a separate (and complex) language spoken between apps that you would need to learn to use. To make matters worse, every app has its own unique dialect or way of speaking these languages. API is hard to use but is powerful and worth considering.

  
You can find our HighLevel Developer Documentation here at <https://developers.gohighlevel.com/>. 

  
Webhooks, on the other hand, are a bit more friendly. They require a triggering event and are used to send information in response to a trigger - such as filling out a form, clicking a link, etc. Compared to API, webhooks require a lot less knowledge to use. Webhooks are a lot easier to use than API, which is why they are recommended before seeking an API connection.

  
You can learn more about webhooks here in this article above.
  
  