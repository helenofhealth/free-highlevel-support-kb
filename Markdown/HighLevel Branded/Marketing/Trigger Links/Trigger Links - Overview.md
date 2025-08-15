**Date Updated:** 2025-07-22T21:05:36.000Z
  
  
Trigger links are a useful method to redirect a user to a specific page after they click on it within an SMS, Email, GMB, FB/IG DM's and WhatsApp. When a user clicks on the trigger link, the system will record it in the contact's activity timeline and trigger a pre-defined action within a workflow. Within the workflow build there are actions and triggers that you can fire off a trigger link click.  
  
  
**Please Note:**

Trigger links are supported in **SMS,** **Email, GMB,and FB/IG/WhatsApp DMs** **ONLY**. 

---

[](#Trigger-links-in-Workflows)

#### [](#Trigger-links-in-Workflows)

[](#Trigger-links-in-Workflows)

#### [](#Trigger-links-in-Workflows)

**Covered in this article**

[**T** **rigger Link use case**](#Trigger-Link-use-cases)

* [Trigger links in Workflows](#Trigger-links-in-Workflows)
* [Trigger links in Campaigns](#Trigger-links-in-Campaigns)

  
[**Trigger Link How-to's**](#Trigger-Link-How-to's)

* [How to use Custom Values and trigger links to change your URL dynamically.](#How-to-use-Custom-Values-and-trigger-links-to-change-your-URL-dynamically.)
* [How to use the Workflow Wait step for a Trigger link Click.](#How-to-use-the-Workflow-Wait-step-for-a-Trigger-link-Click.)
* [How to set up unsubscribe trigger links by communication channels (SMS, Email, GMB, FB/ IG DMs)](#How-to-set-up-unsubscribe-trigger-links-by-communication-channels-%28SMS,-Email,-GMB,-FB/-IG%29)

[**FAQ**](#FAQ)

   * [How do I brand my trigger links?](#How-do-I-brand-my-trigger-links?)
   * [How do I find the contacts' activity timeline?](#How-do-I-find-the-contacts'-activity-timeline?)

####   
  
---

### **Trigger Link Use Cases**

###   

**Dynamic URL Updates in Email Campaigns:**

Use trigger links to dynamically update URLs in your email campaigns. For instance, if you run monthly or quarterly promotions and want to use the same email template, you can set up a trigger link with a custom value that points to the current promotion URL. When a contact clicks on this link, it takes them to the latest promotion page. This way, you can reuse your email template without manually updating the links each time.

  
**Workflow Automation Based on Trigger Link Clicks:**

Set up workflows that respond to trigger link clicks. For example, you can create a workflow that sends appointment confirmations and reminders. When a contact clicks on a trigger link in an appointment reminder email, the system records the click and triggers the next step in the workflow, such as sending a survey or review request.

  
**Unsubscribe Links for Different Communication Channels:**

Implement unsubscribe trigger links for various communication channels, including SMS, Email, Google My Business (GMB), Facebook, and Instagram. A contact who clicks on these links will be unsubscribed from the respective channel. This ensures compliance with opt-out regulations and helps manage communication preferences effectively.

  
**Branding of Trigger Links:**

Customize the appearance of your trigger links to match your agency's branding. By setting up your API domain ([see FAQ below](https://help.gohighlevel.com/support/solutions/articles/48000981404-trigger-links-overview#How-do-I-brand-my-trigger-links?:~:text=FAQ-,How%20do%20I%20brand%20my%20trigger%20links%3F,-To%20set%20up)), you can ensure that trigger links display your agency's domain, providing a more professional and branded experience for your users.

  
**Tracking Contact Activity:**

Use trigger links to track a contact's engagement and actions within your SMS and email campaigns. When a contact clicks on a trigger link, their activity is recorded in the contact's activity timeline. This information can be valuable for assessing their behavior and campaign effectiveness.

  
**Educational Resources in Campaigns:**

Embed trigger links within your email campaigns to provide educational resources. For instance, you can include links to tutorials, how-to videos, or articles related to your products or services. Clicking on these trigger links can trigger automated follow-up actions or track a contact's interest in specific topics.

  
**Event Registration and Updates:**

If you're organizing events, use trigger links in your email invitations. When recipients click on the trigger link to RSVP or get event updates, you can automate the process of confirming their attendance, sending event details, or collecting additional information.

  
**Product Recommendations and Personalization:**

In your email marketing, incorporate trigger links that lead contacts to personalized product recommendations based on their preferences and past interactions. Triggering this link can initiate automated processes to tailor future communications and product offerings.
  
  
---

## **Trigger links in Workflows**

**If you would like to see the continued setup for this workflow, please check out:**

#### [How to use the Workflow Wait step for a Trigger link click](#How-to-use-the-Workflow-Wait-step-for-a-Trigger-link-Click-4)

####   
**Check out this how-to guide:** [Build Automated Appointment Followup Surveys with HighLevel Workflows](https://www.youtube.com/watch?v=Y2v1btMRZUE).
  
  
---

# **Trigger Link How-to's**

##   
**How to use [Custom Values](https://help.gohighlevel.com/en/support/solutions/articles/48001161575) and trigger links to change your URL dynamically.**

  
This is great if you're running promotions monthly or quarterly and want to use the same workflow. Update your _custom value URL_ to point to your new "offer URL," and the system will dynamically update the trigger link. 

  
**Please Note:**

- This will **not** retroactively affect any previous link URLs from past campaigns.  
  
- When setting up your workflow please make sure to add the "**trigger link**" to your SMS or Email message body. Placing the "Custom Value" in the message body will not "**fire**" the trigger link when clicked.

To use a Custom Value with a Trigger Link correctly, first create the Trigger Link in the platform, then assign the dynamic URL (your Custom Value) to that Trigger Link, and finally insert the actual Trigger Link—not the raw Custom Value—into your message body.
  
  
##   
  
**How to use the Workflow Wait step for a Trigger link Click.**

  
This video covers how to use a "wait" step action within a workflow to trigger the next step based on a trigger link click. This workflow can be found in your workflow library as **"Recipe - Appointment Confirmation + Reminder + Survey + Review Request."** 
  
  
## **How to set up unsubscribe trigger links by communication channels (SMS, Email, GMB, FB/ IG DMs)**
  
  
**Please Note:**

By default the **SMS carriers have prebuilt** **opt-out keywords** like **['STOP', 'STOPALL', 'UNSUBSCRIBE', 'CANCEL', 'END', 'QUIT']. W**hen these keywords are used the lead/ contact will automatically be unsubscribed.   
  
To opt back-in the lead/ contact will need to respond **"Start".**
  
  
---

# **FAQ**

  
### **How do I brand my trigger links?**

To set up your API domain to show your agency domain, please [click here: Setting up my agency API Domain](https://help.gohighlevel.com/en/support/solutions/articles/48001143244).  
  
Currently, you **cannot** set each location/subaccount to have its own API domain. You can add one domain that will be shared across all locations/ sub-accounts.
  
  
### **How do I find the contacts' activity timeline?**

Click on contacts **\>** Smartlist **\>** search for the contact > Click on '**activity**'

![](https://s3.amazonaws.com/cdn.freshdesk.com/data/helpdesk/attachments/production/48278188001/original/tQiXvIBFQTalUwiuOZ5oGLSS_7cfaUvxJA.png?1674834637)

  
### **What does the 'Timeout' toggle in the Wait Action do?**

When enabled, the timeout function will skip the Wait Action (step) after the amount of time you define in the input box under the toggle (visible only when it is enabled).

  
![](https://s3.amazonaws.com/cdn.freshdesk.com/data/helpdesk/attachments/production/155018392858/original/mEXMmc4R78gXadRH3AY69KJugOmbEzavsQ.gif?1705957179)

  