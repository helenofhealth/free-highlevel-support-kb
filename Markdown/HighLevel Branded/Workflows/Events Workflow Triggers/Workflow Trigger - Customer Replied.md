**Date Updated:** 2024-12-13T22:53:08.000Z

The **“Customer Replied”** workflow trigger is a powerful tool designed to automate actions based on customer responses. This guide explains how to configure the trigger, the benefits it offers, and examples of practical use cases to streamline your business processes. By the end, you’ll have a clear understanding of how to utilize this trigger effectively.

---

**TABLE OF CONTENTS**

1. [What is the Customer Replied Workflow Trigger?](#What-is-the-Customer-Replied-Workflow-Trigger?)[](#Key-Benefits-of-Using-This-Trigger)
2. [Key Benefits of Using This Trigger](#Key-Benefits-of-Using-This-Trigger)[](#Configuring-the-Trigger%3A-A-Step-by-Step-Process)
3. [Configuring the Trigger: A Step-by-Step Process](#Configuring-the-Trigger%3A-A-Step-by-Step-Process)[](#Use-Cases)
4. [Use Cases](#Use-Cases)[](#FAQs)
5. [FAQs](#FAQs)

---

# **What is the Customer Replied Workflow Trigger?**

  
The **“Customer Replied”** workflow trigger activates a specific workflow when a customer responds to a message. It allows businesses to automate follow-up actions, notifications, or processes tailored to customer interactions, enhancing efficiency and response accuracy.

---

## **Key Benefits of Using This Trigger**

  
1. **Enhanced Automation:** Automatically initiate actions like creating tasks or sending notifications based on customer replies.
2. **Improved Responsiveness:** Ensure timely follow-ups by reacting instantly to customer interactions.
3. **Customizable Filters:** Tailor workflows using filters such as specific phrases, tags, or intent types.
4. **Channel-Specific Workflows:** Customize triggers based on reply channels like WhatsApp or email, ensuring precise automation.

---

## **Configuring the Trigger: A Step-by-Step Process**

  
Start your journey by getting inside the **"Automation"** section of your CRM and click the "Workflows" menu if you're not already there.

![](https://s3.amazonaws.com/cdn.freshdesk.com/data/helpdesk/attachments/production/155038297078/original/UVlh3ZReNi33lMcQlmxgqA4q90llLKyleA.png?1734093976)

  
Click **"+ Create Workflow"** button located at the top right corner. From the dropdown, select **"+ Start from Scratch"** option.

![](https://s3.amazonaws.com/cdn.freshdesk.com/data/helpdesk/attachments/production/155038298163/original/xwZ-VzJ4hJvneWoUi7n4-Ktr8lsvV7uobQ.png?1734094712)  
Now that you are inside the workflow editor, Let's find the **"Customer Replied"** trigger. for that, click "**Add New Trigger"** option and scroll down until you get there.  
![](https://s3.amazonaws.com/cdn.freshdesk.com/data/helpdesk/attachments/production/155038300116/original/T4wg9BhdNE5rhrmPT1DtTnIvFd7geG8Aww.png?1734096024)

  
Let's name this trigger. Use a descriptive name for easy identification.

![](https://s3.amazonaws.com/cdn.freshdesk.com/data/helpdesk/attachments/production/155038300166/original/ZdLhFnqsvGwkdxni8UyhViXOivBm12oNHw.png?1734096061)

  
Add Filters option gives you the ability to set the specific conditions for this trigger to get activated. Click **"+Add Filters."**  
![](https://s3.amazonaws.com/cdn.freshdesk.com/data/helpdesk/attachments/production/155038300221/original/1ifvsRYuU6qR3Tsf1uKPjV3GOtWvGAWang.png?1734096089)

  
Now you can see the multiple filtering options that would match your campaign. Let's understand these filters :

* **Contains Phrase :** Let's you add a phrase so the system can only trigger when the customer's response has the phrase we added in this filter.
* **Doesn't Have Tag :** Use this filter to exclude the contacts from entering into this workflow who have certain tags. Example, you do not want to offer your local service to the contact whose address is outside of your service area. so you may have a contact list with the tag "Austin Texas" and add the tag in this filter so the system should exclude the contacts who are from Austin Texas"
* **Exact Match Phrase :** This filter allows you to enter the exact response that you expect from a contact.
* **Has Tag :** As the name suggests, you can include the contact tags in this filter so the trigger gets activated only when the contact has the Tags you have saved in the filter.
* **Intent Type :** In this filter, the system tries to understand the contact response, if it is positive or negative, then uses this automation as a reply to the contact's response.
* **Replied to Workflow :** When you want to create a hyper targeted campaign for contacts who have previously responded to another workflow you can use this filter to select the workflow and the system will start adding those contacts from the selected workflow to the current workflow.
* **Reply Channel :** This filter gives you the ability to select the contacts based on the reply channel. This way you can choose to add the contacts who have responded to your SMS campaign or Email campaigns.

![](https://s3.amazonaws.com/cdn.freshdesk.com/data/helpdesk/attachments/production/155038300528/original/PfN9hDUCU9amwMtSkL6aDnwzJ8i_rJdAuw.png?1734096273)

  
Below are the few ways you can use filters when configuring the **"Customer Replied"** trigger.

![](https://s3.amazonaws.com/cdn.freshdesk.com/data/helpdesk/attachments/production/155038300254/original/Qnx2nseiBz71bY3ZKHDKjhH6ztGZaAOK1w.png?1734096121)  
Be sure to **"Save"** your changes during each step. When are done setting up the workflow trigger and actions, use the **"Test Workflow"** option before making it Live.

![](https://s3.amazonaws.com/cdn.freshdesk.com/data/helpdesk/attachments/production/155038301125/original/wtA08LwnFC62jiitJ8t4QyM2HttEpDRRwA.png?1734096687)

  
When you are in the middle of creating the workflow, its always in the draft mode. When everything is set up, you will need to use this toggle to publish the workflow.

![](https://s3.amazonaws.com/cdn.freshdesk.com/data/helpdesk/attachments/production/155038297085/original/vaAVrZ1fF9VJiWsOpH5ZgNyF17F_CbZW1A.png?1734093998)

---

## **Use Cases**

1. **Creating Opportunities from Positive Replies:**  
   * **Scenario:** A sales team wants to automatically create a CRM opportunity when a customer replies positively to a proposal.  
   * **Trigger Setup:**  
         * **Trigger:** Customer Replied  
         * **Filters:** Contains phrase: “interested,” “confirm.”  
         * **Workflow Actions:** Create an opportunity in the CRM with the reply details.Notify the sales team about the new opportunity.Send an email to the assigned user for immediate follow-up.  
         * **Outcome:** Timely creation of opportunities to improve lead management.
2. **Customer Support Ticketing:**  
   * **Scenario:** Automate ticket creation when a customer responds with a complaint or question.  
   * **Trigger Setup:**  
         * **Intent Type:** Complaint or Question.  
         * **Filters:** Reply channel: Email.  
         * **Workflow Actions:**Create a support ticket with priority settings.Assign the ticket to the appropriate team.Notify the support team for urgent action.
3. **Post-Purchase Follow-Up:**  
   * **Scenario:** Automate thank-you messages when customers respond positively after a purchase.  
   * **Trigger Setup:**Contains Phrase: “Thanks,” “great.”  
         * **Reply Channel:** WhatsApp.  
         * **Workflow Actions:**Send an automated thank-you message.Request a review or feedback. Log the interaction in the CRM.

---

## **FAQs**

  
 **1\.** **Can I trigger workflows for replies from specific customers only?**

Yes, you can use tags to narrow down workflows to specific customer segments.

  
 **2\.** **How do intent types work with this trigger?**

Intent types use natural language processing (NLP) to categorize replies, such as “question,” “complaint,” or “positive response.” You can then configure workflows to handle each intent appropriately.

  
**3\.** **Can I trigger different workflows based on reply channels?**

Absolutely! You can configure workflows for specific channels like WhatsApp or email, and even narrow it down to particular numbers or addresses.

  