**Date Updated:** 2024-12-30T00:57:21.000Z

# **Zapier Setup Guide - Developer Integration**

  
### To create new subaccounts via Public API please make sure you're currently subscribed to the [ProPlan](https://help.gohighlevel.com/support/solutions/articles/48001208376#Q8%29-How-Do-I-Upgrade-my-HighLevel-Account?).[](https://help.gohighlevel.com/support/solutions/articles/48001208376#Q8%29-How-Do-I-Upgrade-my-HighLevel-Account?)

  
****For more information and links to our API documentation, visit our developer's website: <https://developers.gohighlevel.com/>** 
  
  
 **Important Notes Before Proceeding Further:**

If you would like to automate account creation within HighLevel (without Zapier) please check out the GHL [**SaaS Guide**](https://help.gohighlevel.com/en/support/solutions/articles/48001184920) (Pro Plan Required)  
  
The [Zapier LeadConnector integration](https://zapier.com/apps/leadconnector/integrations) action "**add Account**" was deprecated **21st Feb. 2022** **.** 

  
The steps in this article are for Advanced Integration and for informational purposes only.   
  
While **our support team does not currently service or support either our API or Custom Zapier Integrations** due to their complexities, we have many tools and groups to help you get started and connected! For assistance with **APIs only**, you can join our Developer Council Slack Community here: <https://www.gohighlevel.com/dev-slack>  
  
We also hold a Developer Council Zoom Call once a month (second to last Friday) which you can find on the Events calendar here: <https://www.gohighlevel.com/events>  
  
**For more information and links to our API documentation, visit our developer's website:** **<https://developers.gohighlevel.com/>**

  
In order to use this article, Zapier webhooks are required which are not included in their free plan. Please sign up for a **paid plan**before proceeding further. 

---
  
  
**TABLE OF CONTENTS**

  
#### [1\. Head into your agency settings and grab your Agency API Key](#1.-Head-into-your-agency-settings-and-grab-your-Agency-API-Key)

#### [2\. Once you have copied the Agency API Key, log into Zapier and create a new Zap](#2.-Once-you-have-copied-the-Agency-API-Key,-log-into-Zapier-and-create-a-new-Zap)

#### [3\. Lets jump back into Zapier and create the location zap](#3.-Lets-jump-back-into-Zapier-and-create-the-location-zap)

#### [4\. Hit Continue and run your test](#4.-Hit-Continue-and-run-your-test)

#### [5\. Last step is to create a user, password and add them to the new location](#5.-Last-step-is-to-create-a-user,-password-and-add-them-to-the-new-location)

#### [6\. Hit Continue and run your test](#6.-Hit-Continue-and-run-your-test)

#### [**Troubleshooting**](#Troubleshooting)

#### [Q1) When creating a user I do not receive a password, location or agency API in the Post results?](#Q1%29-When-creating-a-user-I-do-not-receive-a-password,-location-or-agency-API-in-the-Post-results?)

#### [Q2) My webhook is not firing from the workflow](#Q2%29-My-webhook-is-not-firing-from-the-workflow)

  
---

  
## **1\. Head into your agency settings and grab your Agency API Key**

**Step 1.1** **:** To create a new location under your agency you will need to use Agency API Keys. To find your API Keys please head into your **Agency V** **iew -> Settings -> API Keys -> Click to copy API key**

  
**Step 1.2** **:** Save this API Key for later, or come back to this step at the two points in this article when prompted to put this into use! We want to ensure you have an Agency API Key on hand before taking the time to build out the rest of your integration

  
**Please note:**

If you do not see the API key please create a new key by clicking on the "**+ Create New**" button (orange arrow)

  
![](https://s3.amazonaws.com/cdn.freshdesk.com/data/helpdesk/attachments/production/48178848059/original/ecNsGcs-m9uuoDpbuU1fWDPD5tgGpRtWNA.png?1642119401)
  
  
## **2\. Once you have copied the Agency API Key, log into [Zapier](https://zapier.com/app/login) and create a new Zap**

  
**Step 2.1** **:** The first step in your zap will be the action/ event that will trigger Zapier to create the account in HighLevel. This action/event can be a LeadConnector action like; pipeline change, add/ update opportunity etc. ([see all internal actions here](https://zapier.com/apps/leadconnector/integrations)) or we can use Zapier's "capture webhook" action and a workflow to create a new subaccount. 

  
For the example below we will be using Zapier's "**C** **apture webhook**" action . Please copy your webhook URL and proceed to next step (2.2) below.

![](https://s3.amazonaws.com/cdn.freshdesk.com/data/helpdesk/attachments/production/48194925453/original/9hyAddnNsmMmiPGMUm4NIQd1X3jBgZoZcg.gif?1645891175)

  
**Please Note:**

To use Zapier webhooks (premium) please sign up for a **paid plan** **.**
  
  
**Step 2.2:** Next, let's set up a NEW workflow in HighLevel that will execute the Zapier webhook that we just created. 

  
The first step in our workflow is an order form called "Account Creation Form". Next, click on the + and search and select "webhook" action (see image below). 

  
**Once you have setup your form and webhook, please test the webhook before proceeding to the next step. To test your webhook please submit the form at least once with some dummy contact data.**
  
  
![](https://s3.amazonaws.com/cdn.freshdesk.com/data/helpdesk/attachments/production/48178863464/original/zL6mUxu4EGRomcUJsZmORPCWrlIEeWnorw.png?1642133236)

**Please Note:**

If you do not submit the form at least once, Zapier will not have the data it requires for the next step which is creating a new location
  
  
## **3\. Lets jump back into Zapier and create the location zap**

  
###   

### **Step 3.1:** Select webhooks again but this time choose "**Custom Request**" and Select "**POST**" as Action Event.
  
  
### **Step 3.2:** Add the location creation endpoint URL:

[](https://rest.gohighlevel.com/v1/locations)<https://rest.gohighlevel.com/v1/locations>

###   
**Step 3.3:** Leave Data Pass-Through **Empty**
  
  
### **Step 3.4:** Next let's map the "**Data**" with the contact info submitted in Step 2.2.

**Please Note:**

**-** If you do not see any data for the "input fields" please head back to your workflow and submit the form at least once.

  
---

{

 "businessName": "{{Insert\_\_company\_name}}",

 "address": "3500 Deer Creek Road",

 "city": "Palo Alto",

 "country": "US",

 "state": "CA",

 "postalCode": "94304",

 "website": "<https://www.tesla.com>",

 "timezone": "US/Central",

 "firstName": "{{Insert \_\_first\_name}}",

 "lastName": "{{Insert  \_\_last\_name}}",

 "email": "{{Insert \_\_email}}",

 "phone": "{{Insert \_\_Phone}}",

 "settings": {

 "allowDuplicateContact": false,

 "allowDuplicateOpportunity": false,

 "allowFacebookNameMerge": false,

 "disableContactTimezone": false

 },

 "snapshot": {

 "id": "NLCFWNuvs9DLwMsYku3H",

 "type": "vertical"

 },

 "social": {

 "facebookUrl": "<https://facebook.com/groups/XXX>",

 "googlePlus": "<https://groups.google.com/d/XXX>",

 "linkedIn": "<https://www.linkedin.com/groups/XXX/profile>",

 "foursquare": "<https://foursquare.com/groups/XXX>",

 "twitter": "<https://twitter.com/XXX>",

 "yelp": "<https://yelp.com/XXX>",

 "instagram": "<https://instagram.com/XXX>",

 "youtube": "<https://youtube.com/XXX>",

 "pinterest": "<https://pinterest.com/XXX>",

 "blogRss": "<https://rss.xyz.com>",

 "googlePlaceId": "redfdfdere"

 }

}
  
  
### **Step 3.5: (Optional) Add Snapshot ID(s) to Payload** 

If you want to automatically load one or more snapshots to the new accounts you will be creating through this integration, you will need to locate the Snapshot ID for each one to place it in the body of the above payload. Watch the video below for the easiest way to locate a Snapshot ID without using an API call.

  
When adding a snapshot please add your "**Snapshot ID**" and the **"Type"** as either: _Own, Imported, Vertical_

What do the differentsnapshot **"Types"** mean?

**\- Own:** [You created this Snapshot](https://help.gohighlevel.com/en/support/solutions/articles/48000982511)

**\- Imported:** Another Agencies Snapshot

**\- Vertical:** Native HighLevel Snapshots
  
  
### **Step 3.6: Leave Basic Authorization Blank**

  
### **Step 3.7: Adding Authorization Headers**

You will need two Headers for your request to be successfully submitted. An Authorization Header which contains your API Key, and a Content Type Header which tells our API what format the data is being sent in. 

  
First, add "**Authorization**" as your Header title, then type the word "**Bearer**" -> add one space then your Agency API key from the first step in the authorization box. 

  
Hit the + button underneath and add a new header: "**Content-Type"**, then "**application/json**"

  
![](https://s3.amazonaws.com/cdn.freshdesk.com/data/helpdesk/attachments/production/48223503954/original/MKkSO5aobHHTa4OBBLIZhLbYpVNPk-Lq5g.png?1651684704)

**Please Note:**

When adding "**Authorization"** as your Header title, then type the word "**Bearer**" -> add **one** **space** then add your agency API key from the first step
  
  
## **4\. Hit Continue and run your test**

Check to see your "**Post**" results for your new location ID

![](https://s3.amazonaws.com/cdn.freshdesk.com/data/helpdesk/attachments/production/48193279760/original/Tfvh5uOai8c80gDI--86E9P746Yax2ht3A.png?1645579331)

  
**Location ID Note:** Just like you did with Section 3.4, when mapping the Location ID to Step 5 of this Article (The User Creation portion) make sure that you **do not copy and paste** the Location ID highlighted in the screenshot. At this stage, you are simply reviewing to ensure a location was successfully created, and a Location ID in this place is proof of such without having to go into your HighLevel account.   
  
If you copy and paste this Location ID into the next step rather than selecting it from the drop down similar to Section 3.4 Field Mapping, all subsequent User Creations that run through this in the future will be mapped to the Location ID that is pasted in rather than dynamically updating each time a new location is created. 
  
  
## **5\. Last step is to create a user, password and add them to the new location**

**![](https://s3.amazonaws.com/cdn.freshdesk.com/data/helpdesk/attachments/production/48193675898/original/DvazTPRbMEkk7Bm4jlM2iN3s1nE_PTs48Q.gif?1645632660)** 

### **Step 5.1:** Select webhooks again, choosing "**Custom Request**" and Select "**POST**" as Action Event.
  
  
### **Step 5.2:** Add the User Creation endpoint URL:

<https://rest.gohighlevel.com/v1/users/>

### **Step 5.3:** Leave Data Pass-Through **Empty**
  
  
### **Step 5.4:** Next let's map the User "**Data**" with the contact info submitted in Step 2.2.

Once you have mapped your input fields from the previous step, make sure to set your desired user permissions.

**![](https://s3.amazonaws.com/cdn.freshdesk.com/data/helpdesk/attachments/production/48194086155/original/JkkYWvOPrNhUYes-39l_ARAf1wNSuVmXwA.png?1645707292)**

**Please Note:**

Leave Password Field Blank to **AUTO Generate a password**.   **OR**  Use 8 characters w/ special Symbols

  
**Location ID:** Note how the Location ID looks in this screenshot. It has been properly mapped from the available list of variables from the previous step as opposed to being copied and pasted into this line.   
  
You will look for the field titled 'ID' 

  
### **User Data Fields: ([Click here to see the developer's docs](https://developers.gohighlevel.com/))**

{

 "firstName": "Zapier",

 "lastName": "Test",

 "email": "test@testing.com",

 "password": "Qwerty123!@#",

 "type": "account",

 "role": "admin",

 "locationIds": \[

 "ABXfgmOjNw2FG2Y4UJPt"

 \],

 "permissions": {

 "campaignsEnabled": false,

 "campaignsReadOnly": false,

 "contactsEnabled": true,

 "workflowsEnabled": true,

 "triggersEnabled": false,

 "funnelsEnabled": false,

 "websitesEnabled": false,

 "opportunitiesEnabled": false,

 "dashboardStatsEnabled": true,

 "bulkRequestsEnabled": true,

 "appointmentsEnabled": true,

 "reviewsEnabled": true,

 "onlineListingsEnabled": true,

 "phoneCallEnabled": true,

 "conversationsEnabled": true,

 "assignedDataOnly": false,

 "adwordsReportingEnabled": false,

 "membershipEnabled": false,

 "facebookAdsReportingEnabled": false,

 "attributionsReportingEnabled": false,

 "settingsEnabled": true,

 "tagsEnabled": true,

 "leadValueEnabled": true,

 "marketingEnabled": true

 }

}

---

### **Step 5.5: Leave Basic Authorization Blank**

  
### **Step 5.6: Adding Authorization Headers**

You will need two Headers for your request to be successfully submitted. An Authorization Header which contains your API Key, and a Content-Type Header which tells our API what format the data is being sent in. 

  
First, add "**Authorization**" as your Header title, then type the word "**Bearer**" -> add one space then your Agency API key from the first step in the authorization box. 

  
Hit the + button underneath and add a new header: "**Content-Type"**, then "**application/json**"

  
![](https://s3.amazonaws.com/cdn.freshdesk.com/data/helpdesk/attachments/production/48223503789/original/b8O8E4RypkwsUDtrMQ_pdVIKCT7OOS6rbQ.png?1651684648)

  
**Please Note:**

When adding "**Authorization"** as your Header title, then type the word "**Bearer**" -> add **one** **space** then add your agency API key from the first step

## **6\. Hit Continue and run your test**

That's it! You have just created a new location and added a user to it
  
  
#   
  
**Troubleshooting**

  
When creating integrations with HighLevel, it is important to understand that you are working with our API regardless of the interface. Whether you are using Zapier, Pabbly Connect, API Nation, Make (Formerly Integromat)or another plug-and-play integrator, these platforms are simply an easier way of utilizing our API to connect multiple platforms, in some cases without any coding experience whatsoever. 

  
Is something not working? **Before doing** **anything else**, pause here and review the following article: [How to use Webhook.site to Troubleshoot my API-related Requests](https://help.gohighlevel.com/support/solutions/articles/48001212085-how-to-use-webhook-site-to-troubleshoot-your-api-requests). 

 \- Review the payload data with your developers and your issue will likely be resolved.

 \- In the event that your issue is still not resolved after reviewing the data and consulting with your development team, feel free to reply back to us with the requested information in the above-listed Webhook.site article and we can review the Webhook data and potentially tell you what is causing your error. 

  
The above is **the first step** in having us review your integration. Without the Webhook.site data, our developers will be unable to isolate the issue you are reporting

  
#### **Q1) When creating a user I do not receive a password, location or agency API in the Post results?**

The system will only generate one unique password per email/phone number. Please make sure when testing that you are using unique data (email/Phone) every time

  
#### **Q2) My webhook is not firing from the workflow**

Please make sure the webhook is live/ published, then recreate the contact using NEW contact info (Unique email/phone). You can append +1 to the current email you were using Ex: myemail+1@gmail.com, myemail+2@gmail.com ect. This will also send any automation emails to the original email... [more info](https://www.google.com/search?q=adding+%2B1+to+my+email&rlz=1C1VDKB%5FenUS938US939&ei=TWQWYpXXD4bCkPIPu9iKiAQ&ved=0ahUKEwjVse%5Ffopb2AhUGIUQIHTusAkEQ4dUDCA4&uact=5&oq=adding+%2B1+to+my+email&gs%5Flcp=Cgdnd3Mtd2l6EANKBAhBGABKBAhGGABQAFieHGCnHWgAcAF4AIAB8gGIAf0OkgEGMTYuMi4xmAEAoAEBwAEB&sclient=gws-wiz)

  
**Please Note:** 

The steps in this article are for Advanced Integration and for informational purposes only.   
  
While **our support team does not currently service or support either our API or Custom Zapier Integrations** due to their complexities, we have many tools and groups to help you get started and connected! For assistance with **APIs only**, you can join our Developer Council Slack Community here: <https://www.gohighlevel.com/dev-slack>  
  
We also hold a Developer Council Zoom Call once a month (second to last Friday) which you can find on the Events calendar here: <https://www.gohighlevel.com/events>  
  
**For more information and links to our API documentation, visit our developer's website:** **<https://developers.gohighlevel.com/>**
  
  