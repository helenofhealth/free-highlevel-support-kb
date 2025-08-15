**Date Updated:** 2025-02-18T18:39:14.000Z

The **Drip Action** in workflows helps regulate the flow of contacts by processing them in batches at set intervals. This prevents overwhelming your system, ensures smooth automation execution, and maintains resource efficiency. In this guide, we’ll walk you through how to configure and optimize the Drip Action for better workflow control.

---

**TABLE OF CONTENTS**

* [What is the Drip Workflow Action?](#What-is-the-Drip-Workflow-Action?)
* [Key Benefits of the Drip Workflow Action](#Key-Benefits-of-the-Drip-Workflow-Action)
* [Configuring Drip Workflow Action](#Configuring-Drip-Workflow-Action)
* [Frequently Asked Questions](#Frequently-Asked-Questions)

---

# **What is the Drip Workflow Action?**

  
The Drip Workflow Action is designed to control the rate at which contacts progress through a workflow by processing them in batches at predefined intervals. Instead of executing actions on all contacts simultaneously, this feature allows you to stagger executions, ensuring smooth automation and preventing system overload. It is especially useful for managing high-volume workflows, such as bulk email or SMS campaigns, where controlled delivery is crucial for maintaining engagement and avoiding resource bottlenecks.

---

## **Key Benefits of the Drip Workflow Action**

  
* **Controlled Execution:** Prevents system overload by processing contacts in manageable batches rather than all at once.

  
* **Optimized Resource Management:** Helps maintain API limits, email/SMS sending capacity, and server performance.

  
* **Improved Deliverability & Engagement:** Spreads out communications over time to avoid spam filters and enhance response rates.

  
* **Flexible Scheduling:** Allows customization of batch size and intervals (minutes, hours, days) for precise automation control.

---

## Configuring Drip Workflow Action
  
  
### **Step 1: Access the Workflow Builder**

  
Log in to your HighLevel account, go to Automation > Workflows, and either create a new workflow or choose an existing one to edit.

  
![](https://s3.amazonaws.com/cdn.freshdesk.com/data/helpdesk/attachments/production/155041803410/original/QlJnd7snzQ_lSrH1OVpWthrur0fxylvbjA.png?1739882387)
  
  
### **Step 2: Add the Drip Action**

  
Click the + icon to add a new action in your workflow, then search for Drip in the action list and select it.

  
![](https://s3.amazonaws.com/cdn.freshdesk.com/data/helpdesk/attachments/production/155041803595/original/F1Jy7GRiPtrofk-I6GyKVI5uxHCPKK51yw.png?1739882507)
  
  
### **Step 3: Naming the Action**

  
Give your Drip action a clear and descriptive name to make it easily identifiable in the workflow builder.

  
![](https://s3.amazonaws.com/cdn.freshdesk.com/data/helpdesk/attachments/production/155041803638/original/k95WlZuhQux8c-6jFbS7nFftWFkS8n-e3w.png?1739882532)
  
  
### **Step 4: Setting the Batch Size**

  
Set the batch size to control how many contacts will move to the next step at a time. You can choose any number between 1 and 10,000, depending on your workflow needs. For example, if you set the batch size to 100, then 100 contacts will proceed at each interval, ensuring a steady and manageable workflow execution.

###   

![](https://s3.amazonaws.com/cdn.freshdesk.com/data/helpdesk/attachments/production/155041806001/original/-DyEvE0byzhzTJHtG2SjeW7_lKKHvFPUUA.png?1739884042)

  
### **Step 5: Configuring the Drip Interval**

  
Set the drip interval to determine how often each batch of contacts will move to the next step. You can choose from minutes (1–60), hours (1–24), or days (1–7) based on your workflow timing needs. For example, if you set the interval to 30 minutes, a new batch of contacts will progress every 30 minutes, ensuring a controlled and consistent workflow execution.

  
![](https://s3.amazonaws.com/cdn.freshdesk.com/data/helpdesk/attachments/production/155041806047/original/xO_eubmcJ3gzBVumg9Pg4U1GHxzRTTNwfA.png?1739884065)
  
  
### **Step 6: Save and Publish the Workflow**

1. Click Save to apply the Drip action settings.
2. Ensure the workflow is properly configured, then click Publish to activate automation.
3. Run a test by adding test contacts and verifying batch processing in workflow history.

---

## **Frequently Asked Questions**

  
**Q: How is the Drip action different from a normal delay or wait step?**

A standard wait step holds all contacts at a specific point in the workflow until the set time passes. In contrast, the Drip action releases contacts in batches, allowing a controlled flow instead of moving everyone forward at once.
  
  
**Q: What happens if my batch size is too large?**

If your batch size is too large, all contacts will move at once, which may overload communication channels (e.g., sending thousands of emails or SMS at once). It’s best to choose a manageable batch size based on your business needs and provider limits.
  
  
**Q: Can I use the Drip action with emails, SMS, and other workflow actions?**

Yes! The Drip action can be used with any workflow step, including emails, SMS, task assignments, and other automation actions, making it a flexible tool for pacing workflow execution.
  
  
**Q: What happens if new contacts enter the workflow while the Drip action is running?**

New contacts will start from the beginning of the workflow and follow the same batch processing rules set in the Drip action. They won’t join an already running batch but will follow their own drip schedule based on the configured settings.
  
  
**Q: Can I change the batch size or drip interval after the workflow is published?**

Yes, you can update the batch size and drip interval at any time. However, changes will only apply to contacts that enter the Drip action after the update. Contacts already in progress will continue following the previous settings.