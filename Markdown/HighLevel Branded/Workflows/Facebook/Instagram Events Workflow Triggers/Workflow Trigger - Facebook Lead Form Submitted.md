**Date Updated:** 2025-04-24T19:03:53.000Z

Easily automate your follow-ups and lead nurturing with the Facebook Lead Form Submitted workflow trigger. This guide walks you through everything you need to know—from setup to best practices—so you can seamlessly connect your Facebook lead generation campaigns with your CRM workflows. Whether you’re launching campaigns or capturing leads across different pages, this automation helps ensure no lead slips through the cracks.

---

**TABLE OF CONTENTS**

* [What is Facebook Lead Form Submitted Workflow Trigger](#What-is-Facebook-Lead-Form-Submitted-Workflow-Trigger)
* [Key Benefits of Facebook Lead Form Submitted Workflow Trigger](#Key-Benefits-of-Facebook-Lead-Form-Submitted-Workflow-Trigger)
* [Configuring Facebook Lead Form Submitted Workflow Trigger](#Configuring-Facebook-Lead-Form-Submitted-Workflow-Trigger)
* [Frequently Asked Questions](#Frequently-Asked-Questions)

---

# **What is Facebook Lead Form Submitted Workflow Trigger**

  
The Facebook Lead Form Submitted trigger is used to initiate a workflow when a lead submits a form through your connected Facebook Page’s Lead Ad. These forms, sometimes called “instant forms,” live natively inside Facebook and don’t require a separate landing page. When a user fills out a form, their data is automatically sent to HighLevel, where you can build automations around follow-ups, tagging, opportunity management, and more.

  
It’s an essential tool for marketers running lead generation ads on Facebook. Instead of manually importing lead data, this trigger handles that for you—firing workflows in real-time based on actual lead submissions.

---

## **Key Benefits of Facebook Lead Form Submitted Workflow Trigger**

  
* **Connect Facebook campaigns directly with CRM automations:** Automatically funnel leads into your workflows without requiring a landing page or manual exports.

  
* **Save time with real-time automation:** Once a user submits the form, they’re immediately added to your CRM—no delays.

  
* **Accurate targeting with filters:** Trigger actions only for specific pages and forms using built-in filters.

  
* **Boost team efficiency:** Assign contacts, notify users, and organize leads into pipelines automatically.

  
* **Create personalized experiences:** Follow up with tailored emails, tags, or pipeline stages based on the lead’s source form.

---

## **Configuring Facebook Lead Form Submitted Workflow Trigger**

  
To set up this trigger, you must first ensure your Facebook account and Lead Forms are integrated and mapped with HighLevel. Follow the steps below to configure the trigger in your workflow:
  
  
### **Add the Trigger to Your Workflow**

  
Navigate to Automation > Workflows and either create a new workflow or edit an existing one. In the workflow builder, click + Add New Trigger to get started.

  
![](https://s3.amazonaws.com/cdn.freshdesk.com/data/helpdesk/attachments/production/155045603059/original/10eJkp9-mjOeEXoS2sltLvqvKzd8PKDqew.jpeg?1745500078)
  
  
### **Choose the Trigger Type**

  
From the list of available triggers, scroll to the Events section and select Facebook Lead Form Submitted. This option appears with a green clipboard icon.

  
![](https://s3.amazonaws.com/cdn.freshdesk.com/data/helpdesk/attachments/production/155045603090/original/ufXsWG0V3Gqos8hDB2p8x4GeF01_KybLPQ.png?1745500118)
  
  
### **Name Your Trigger**

  
Provide a descriptive name in the Workflow Trigger Name field. This helps you identify the trigger later, especially if you’re managing multiple lead sources. Example: Facebook Lead Form Submitted (Weight Loss Campaign)

  
![](https://s3.amazonaws.com/cdn.freshdesk.com/data/helpdesk/attachments/production/155045603110/original/A32rsx8iJ9UG70fmp3HNbFzsbutGpFIQTw.jpeg?1745500138)
  
  
### **Apply Filters to Target the Right Audience**

  
After naming the trigger, add filters to ensure only leads from the correct Facebook Page and Form trigger the workflow.

  
**Page Is:** Select the Facebook Page running the campaign. Only connected pages from Settings > Integrations > Facebook will appear here.

  
![](https://s3.amazonaws.com/cdn.freshdesk.com/data/helpdesk/attachments/production/155045603339/original/G9DpwHbhpYto224xX4imixdNDgPuC8o4gg.jpeg?1745500227)
  
  
**Form Is**

  
After choosing a Page, this filter lets you select a specific Lead Form associated with it.

  
![](https://s3.amazonaws.com/cdn.freshdesk.com/data/helpdesk/attachments/production/155045603279/original/op16hb90SYlcTQ4UaCvEYOBXQ0qLgnfuwQ.jpeg?1745500201)
  
  
### **Save and Build the Workflow**

  
Once your trigger and filters are configured, click **Save Trigger** and begin building your workflow logic. 

After defining all the necessary actions, be sure to **Test Workflow** to confirm everything works as expected, and finally, **Publish** the workflow to activate it.
  
  
**Recommended Workflow Actions for Facebook Leads**
Once your Facebook Lead Form Submitted trigger is set, consider these best practices to streamline lead management and boost response times:

**Create/Update Opportunity:** Automatically route new leads into your sales pipeline to keep things organized.

**Assign to User:** Ensure each lead is immediately owned by a team member for faster follow-up.

**Send Email:** Deliver a personalized thank-you or welcome email to keep the lead engaged from the start.

**Internal Notification:** Alert your team in real-time whenever a new lead enters the system, so no opportunity goes unnoticed.

These steps help you respond quickly and build stronger engagement with every lead that comes through your Facebook campaigns.

---

## **Frequently Asked Questions**

  
**Q: What happens if I don’t use any filters in the trigger setup?**

If no filters are applied, the workflow will trigger for any Lead Form submitted across all connected Facebook Pages. This might result in undesired workflows firing, so it’s best practice to use filters like “Page Is” and “Form Is.”

  
**Q: Do I need to map Facebook Lead Form fields before setting this up?**

Yes. Go to Settings > Integrations > Facebook Form Fields Mapping and ensure your lead form fields (e.g., name, email, phone) are mapped to HighLevel contact fields. Without proper mapping, lead data may not sync correctly.

  
**Q: Why don’t I see my Facebook Pages or Forms in the dropdown?**

This usually happens when the Facebook integration hasn’t been completed. Make sure your Facebook Page is connected under Settings > Integrations > Facebook, and the correct permissions are granted.

  
**Q: Can I trigger a workflow from multiple Facebook forms in the same trigger?**

No, the trigger supports one form per filter setup. However, you can either clone the trigger inside the same workflow with different filters or set up separate workflows for each form.

  
**Q: What actions can I automate after a form is submitted?**

Common actions include sending confirmation emails, assigning leads to users, tagging contacts, creating opportunities in pipelines, and sending internal team notifications. You can stack as many steps as you need.