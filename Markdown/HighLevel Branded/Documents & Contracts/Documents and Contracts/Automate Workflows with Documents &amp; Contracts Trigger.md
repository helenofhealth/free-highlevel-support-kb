**Date Updated:** 2025-07-25T21:43:28.000Z

This article explains how to use the “Documents & Contracts” workflow trigger to automate actions based on document status. Whether a document is sent, signed, viewed, or completed, this trigger allows you to kick off automated workflows like sending notifications, tagging contacts, or updating pipelines. You can also filter workflows by template, recipient type, or document values to create highly specific automation paths. This is especially useful for managing proposals, NDAs, and signed agreements more efficiently.

---

**TABLE OF CONTENTS**

* [What is Documents & Contracts Workflow Trigger?](#What-is-Documents-&-Contracts-Workflow-Trigger?)
* [Key Benefits of Documents & Contracts Workflow Trigger](#Key-Benefits-of-Documents-&-Contracts-Workflow-Trigger)
* [How to Configure the Documents and Contracts Workflow Trigger](#How-to-Configure-the-Documents-and-Contracts-Workflow-Trigger)
* [Frequently Asked Questions](#Frequently-Asked-Questions)

---

---

# **What is Documents & Contracts Workflow Trigger?**

  
The **Documents & Contracts workflow trigger** in HighLevel is designed to automate actions when the status of a document changes—such as when it’s sent, viewed, signed, or completed. This trigger connects the document lifecycle to your workflow automation, allowing you to take action instantly based on recipient interactions. It’s ideal for streamlining communication, record-keeping, and follow-up tasks tied to proposals, agreements, or contracts.

  
This trigger is especially useful for **agencies, service providers, and businesses** that regularly send documents for signature or approval. By enabling filters like **Status, Template Name, and Recipient Type**, users can build highly targeted workflows that match specific scenarios. Whether you’re managing NDAs, sales proposals, or contracts, this trigger helps keep your processes organized, timely, and scalable.

---

## **Key Benefits of Documents & Contracts Workflow Trigger**

  
This workflow trigger gives users the ability to automate document-based tasks with precision. Whether you’re tracking signatures or customizing follow-up based on document status, the trigger enhances operational efficiency and communication.

  
* **Automated Follow-Up Based on Document Status:** Trigger personalized workflows when a document is sent, viewed, signed, or completed—ensuring timely reminders, updates, or internal actions without manual tracking.

  
* **Improved Record Management:** Automatically update CRM fields, Google Sheets, or Slack channels based on document activity to keep your records up to date and eliminate data entry errors.

  
* **Dynamic Filtering for Targeted Automation:** Use filters like Template Name, Status, and Recipient Type to trigger workflows only for specific documents or recipients—perfect for managing multiple document types with different workflows.

  
* **Enhanced Internal Team Collaboration:** Send instant internal notifications when key actions are taken on a document, allowing sales or operations teams to follow up or take the next step without delay.

  
* **Personalized Client Experience:** Use custom values from the contact or document to personalize outgoing emails, notifications, or actions—helping you maintain a professional and client-focused communication flow.

---

## **How to Configure the Documents and Contracts Workflow Trigger**

  
### **Navigate to Automation**

  
From the left-hand navigation panel, click on Automation, then select the blue + Create Workflow button on the top-right. Choose Start from Scratch to build a custom workflow.

  
![](https://s3.amazonaws.com/cdn.freshdesk.com/data/helpdesk/attachments/production/155050138126/original/JDTNUOmFqwSypcTAt4onvzkPLr16UZYjKA.png?1753084464)  

  
### **Add a New Trigger**

  
Inside the workflow builder, click + Add New Trigger to set your entry condition. In the trigger list, scroll to the Payments section and click Documents & Contracts. This will trigger the workflow when a document-related event occurs.

  
![](https://s3.amazonaws.com/cdn.freshdesk.com/data/helpdesk/attachments/production/155050138163/original/YxYmN0at4n7IVWc8FZT1sZ3_UUpytUUDlg.png?1753084486)  

  
### **Name Your Trigger**

  
For organizational clarity, give your trigger a specific name (e.g., “Contract Viewed – Onboarding Doc”) in the Workflow Trigger Name field.

  
![](https://s3.amazonaws.com/cdn.freshdesk.com/data/helpdesk/attachments/production/155050138195/original/vJVVL0mNv_ugyeTIv2cmmVIEJS0elB5bfA.png?1753084509)
  
  
### **Add Filters**

  
Click Add Filters to set the specific conditions that determine when the workflow should trigger.

  
![](https://s3.amazonaws.com/cdn.freshdesk.com/data/helpdesk/attachments/production/155050138353/original/B5B6W4cjjAM8SSaIxCGuduxgzRV3tgktRQ.png?1753084634)
  
  
### **Choose Filter Fields and Conditions**

  
You can choose from the following standard filters:

  
* **Recipient Type:** Contact or Business User

  
* **Status:** Viewed, Signed/Accepted, Completed, Sent

  
* **Template:** Specific document template

  
* **Value:** Contract value, useful for high-ticket filtering

  
![](https://s3.amazonaws.com/cdn.freshdesk.com/data/helpdesk/attachments/production/155050138365/original/EQOWr2EwHhRQd6Dt3cVXCa5rEpoyl2Cqcg.png?1753084655)
  
  
### **Recipient Type Filter**

  
Use the “Recipient Type” filter to specify who the document was sent to—either a Business User or a Contact. This ensures your workflow only triggers based on actions taken by the intended recipient type.

  
![](https://s3.amazonaws.com/cdn.freshdesk.com/data/helpdesk/attachments/production/155050138662/original/VomGMNsKJ5LWh2AaOrDYbMYcb_uBxHwkpw.png?1753084845)
  
  
### **Status Filter**

  
The “Status” filter lets you trigger workflows based on the stage of the document—such as when it’s Sent, Viewed, Signed/Accepted, or Completed. This allows you to tailor automation to specific actions taken on the document.

  
![](https://s3.amazonaws.com/cdn.freshdesk.com/data/helpdesk/attachments/production/155050138722/original/S8VozLTPqiGht7et4f0satCACVzNu73wXQ.png?1753084893)
  
  
### **Template Filter**

  
The “Template” filter allows you to specify which document or contract template should trigger the workflow. This is useful when you want automations to run only for certain agreements, such as onboarding forms or service contracts.

  
![](https://s3.amazonaws.com/cdn.freshdesk.com/data/helpdesk/attachments/production/155050138775/original/vknXb90h7z_GqRa0OvZXn10dt42YcOt6sg.png?1753084950)
  
  
### **Value Filter**

  
The “Value” filter lets you trigger workflows based on the monetary amount or numerical value assigned to a document. You can apply operators like “Greater than” or “Equals to” to run automations only when documents meet specific value conditions—ideal for contracts tied to budget thresholds or pricing tiers.

  
![](https://s3.amazonaws.com/cdn.freshdesk.com/data/helpdesk/attachments/production/155050138918/original/w6QjbwMT4mYadLEMbtRno0WL83220eqGbQ.png?1753085030)  

  
### **Save Your Trigger**

  
Once your filters are set, click Save Trigger to apply the configuration. Your workflow will now automatically activate based on document events that match the criteria you’ve defined.

  
![](https://s3.amazonaws.com/cdn.freshdesk.com/data/helpdesk/attachments/production/155050138603/original/U47aDMa6KtUVMvs9RZFdsjNAMMF2jbcirA.png?1753084817)

---

## **Frequently Asked Questions**

  
**Q: Can I trigger different workflows based on whether a document was signed by a Contact versus a Business User?**

Yes. Using the **Recipient Type filter**, you can choose whether the trigger applies to **Contacts** (external users like leads or clients) or **Business Users** (team members or staff). This is especially useful when you need to run separate workflows for client-facing agreements versus internal approvals. For example, you could send a client onboarding email if a Contact signs a proposal, but trigger an internal Slack alert if a Business User signs off on an internal review document.

  
**Q: What happens if the same document is both viewed and signed—will the trigger fire twice?**

Yes. Each **status change** (e.g., from “Viewed” to “Signed/Accepted”) is treated as a separate event and can independently activate the workflow if both statuses are configured as triggers. To avoid redundant automations, you should **add conditional logic** inside your workflow to check for tags or custom field values before executing actions. This prevents overlapping messages or updates.

  
**Q: Can I use the “Value” filter to trigger workflows only for high-ticket contracts, like proposals above $5,000?**

Absolutely. The **Value filter** allows you to apply operators such as “Greater than” or “Equals to.” You can configure your trigger to only activate when the contract’s value exceeds a specific threshold. This is particularly useful for sending different onboarding steps for high-value clients or notifying sales managers about large deals.

  
**Q: How do I restrict workflows to only trigger for specific document templates (e.g., NDAs or service agreements)?**

Use the **Template filter** to select which specific document templates should activate the workflow. This allows you to run unique automations tied to individual document types. For instance, you might send a welcome sequence for clients who signed a “Service Agreement” template, but a different sequence for those who completed a “NDA” template. This ensures workflows are **context-specific** and only trigger when the exact template is used.