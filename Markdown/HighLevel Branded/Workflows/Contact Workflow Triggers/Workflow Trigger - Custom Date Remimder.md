**Date Updated:** 2025-01-21T18:24:21.000Z

The Custom Date Reminder Workflow Trigger is designed to help businesses automate reminders and notifications based on specific custom dates, such as anniversaries, subscription renewals, or event reminders. This trigger ensures that timely follow-ups are sent out, improving customer experience and operational efficiency. In this article, you’ll learn what the trigger is, its key benefits, how to configure it, and answers to common questions users may have.

---

**TABLE OF CONTENTS**

* [What is Custom Date Reminder Workflow Trigger?](#What-is-Custom-Date-Reminder-Workflow-Trigger?)
* [Key Benefits of Custom Date Reminder Workflow Trigger](#Key-Benefits-of-Custom-Date-Reminder-Workflow-Trigger)
* [Configuring the Custom Date Reminder Workflow Trigger](#Configuring-the-Custom-Date-Reminder-Workflow-Trigger)  
   * [Naming a Workflow Trigger](#Naming-a-Workflow-Trigger)  
   * [Add Filters](#Add-Filters)  
   * [Match on Year Along with Day and Month](#Match-on-Year-Along-with-Day-and-Month)  
   * [Custom Date Field Filter](#Custom-Date-Field-Filter)  
   * [Advanced Filters](#Advanced-Filters)
* [Frequently Asked Questions](#Frequently-Asked-Questions)

---

# **What is Custom Date Reminder Workflow Trigger?**

  
The Custom Date Reminder Workflow Trigger activates a workflow on a specific date set within a custom field in your CRM. This trigger is useful for automating processes that rely on custom dates, such as sending out reminders before or after important dates like customer birthdays or contract renewal dates. You can customize the trigger by adding filters to control when and how it should activate.

---

## **Key Benefits of Custom Date Reminder Workflow Trigger**

  
* **Improves Customer Engagement:** Ensures timely communication by sending reminders or follow-ups based on relevant dates.
* **Highly Customizable:** Allows users to add filters and specify triggers for exact dates, days before or after the custom date, and even specific months.
* **Supports Compliance and Proactivity:** Helps businesses stay proactive in client relationship management, such as contract renewals or service reminders.
* **Reduces Manual Workload:** Automates repetitive tasks, saving time and reducing the risk of missing critical dates.

---

## **Configuring the Custom Date Reminder Workflow Trigger**

  
Let’s learn how to select the appropriate custom date fields, configure filters like “After Number of Days” or “Day Is,” and define actions tailored to your business needs. We will also cover the steps to set up the trigger to activate precisely on the specified dates, streamlining the automation of reminders, follow-ups, and other date-driven tasks.

  
### **Navigating to Workflow Builder**

  
Head over to the **"Automation"** section and select **“+ Create New Workflow.”** Choose **“Start from Scratch”** to build a workflow from the ground up or **“Select a Template”** to customize pre-built options available in the system. If you wish to add this trigger to an existing workflow, locate the desired workflow, hover over it, and select it to begin editing..

  
![](https://s3.amazonaws.com/cdn.freshdesk.com/data/helpdesk/attachments/production/155040111408/original/Gqovi-DbLC4Udzz7Ar-K8iDpgp4wAyZbVQ.png?1737369481)
  
  
### **Add a New Workflow Trigger**

  
To start setting up the trigger,” click the **“Add New Trigger”** button and select **"Custom Date Reminder"**  from the list of available options. 

  
![](https://s3.amazonaws.com/cdn.freshdesk.com/data/helpdesk/attachments/production/155040110969/original/0pCxJxs0VzChGXOqTkFb-cdnrdP_c2aklg.jpeg?1737369179)

  
### **Naming a Workflow Trigger**

  
Assign a descriptive name to your trigger for easy identification. A clear name ensures that your workflows remain organized and simplifies locating specific triggers for future updates.

  
![](https://s3.amazonaws.com/cdn.freshdesk.com/data/helpdesk/attachments/production/155040111663/original/mnOenB8Nq-DqxTVfkV9cYIlX5rRMiGoLCQ.png?1737369635)

  
### **Add Filters**

  
The “Add Filters” button opens a list of available filters that can be added to your trigger.

  
![](https://s3.amazonaws.com/cdn.freshdesk.com/data/helpdesk/attachments/production/155040116971/original/eBXF1KpkllZEOYWMyeUwxTUX9hM2yJwdxQ.png?1737373413)
  
  
### **Match on Year Along with Day and Month**

  
Enabling this option ensures the trigger activates only when the year in the custom date field matches the current year. This is particularly useful for date-specific workflows, such as annual reminders or time-sensitive follow-ups, where the exact year is crucial.

  
![](https://s3.amazonaws.com/cdn.freshdesk.com/data/helpdesk/attachments/production/155040122043/original/zqSZXLQFJxGKmnI1JSv9hAwrX60hVuV5PQ.png?1737376743)
  
  
#### **Custom Date Field Filter**

  
The custom date field filter lets you choose specific custom date fields that will activate the workflow. It ensures the workflow is tied to a particular date field that holds critical, time-sensitive information such as proposed appointment time, birth date, policy expiry date.

  
* **Birthday :** Represents a simplified format of a contact’s birthday, typically Month and Day (MM/DD). It’s commonly used when the year is not necessary.
* **Birthday (MM/DD/YYYY) :** Stores the full birth date, including the year. This option is essential for workflows that need to calculate or validate the contact’s exact age.
* **Policy Expiry Date :** Tracks the expiration date of a customer’s policy. It’s vital for businesses like insurance providers or subscription-based services to ensure renewals are handled on time.
* **Policy Purchase Date :** Logs the date when a customer purchased a policy. It helps businesses track anniversaries or follow-up schedules based on the purchase date.
* **Proposed Appt Time :** Refers to the date and time of a scheduled appointment. This field is crucial for workflows that involve scheduled customer interactions, such as consultations or services.

  
![](https://s3.amazonaws.com/cdn.freshdesk.com/data/helpdesk/attachments/production/155040122155/original/9vUlahCim3PHP0lMIHWdRw-mdLlSN7xd3A.png?1737376830)
  
  
### **Advanced Filters**

  
* **After Number of Days :** This filter allows you to set the trigger to activate a specific number of days after the custom date. For example, if the custom date is a policy purchase date, setting this filter to five days ensures the workflow activates on the fifth day after the purchase. It’s perfect for follow-ups or reminders post-event.
* **Before Number of Days:** With this filter, you can configure the workflow to activate a certain number of days before the custom date. For instance, you can send a reminder email three days before a policy expiry date or a scheduled appointment, ensuring timely action or preparation.
* **Has Tag :** This filter narrows down the trigger’s activation to contacts with a specific tag in the CRM. Tags can be used to customize workflows for specific customer segments, adding precision to your automation.
* **Day Is:** This filter lets you specify an exact day (e.g., Monday, Tuesday) for the workflow to trigger. It’s especially useful for scheduling tasks or actions on a particular day of the week, like setting a follow-up call or initiating a promotional campaign on a specific weekday.
* **Month Is:** Use this filter to define the workflow activation for a particular month (e.g., June, December). It’s ideal for planning seasonal campaigns, sending birthday messages, or initiating actions related to recurring annual events.

  
![](https://s3.amazonaws.com/cdn.freshdesk.com/data/helpdesk/attachments/production/155040127086/original/fYemuwNmKdFAFt43Nnbr9R6yOr6IvwK6LQ.png?1737380020)

  
### **Save and Publish the Workflow**

  
Saving your progress while building a workflow is crucial to ensure you don’t lose your adjustments and can pick up right where you left off. Additionally, once your workflow is complete and ready to function, don’t forget to toggle it from **“Draft”** to **“Publish”** to activate it.

---

## **Frequently Asked Questions**

**Q. How do I set up reminders for multiple dates using this trigger?**

You can set up multiple workflows for different custom date fields, each triggering a unique reminder. Ensure each workflow is properly named and configured to avoid confusion.
  
  
**Q. Can I trigger reminders before and after the custom date simultaneously?**

Yes, you can set up two separate triggers—one for reminders before the date and another for reminders after the date within the same workflow.
  
  
**Q. What happens if the custom date field is empty for a contact?**

The trigger will not activate for contacts without a value in the custom date field. Ensure all relevant contacts have dates set in their custom fields.
  
  
**Q. Can I use this trigger to send recurring annual reminders?**

Yes, you can enable the **“Match on the year along with the day and month”** option to ensure the trigger fires every year on the same date.

  
**Q. How can I ensure the trigger only activates for specific contacts?**

Use filters like **“Has Tag”** or **“Business Niche”** to narrow down the trigger to specific groups of contacts.

  