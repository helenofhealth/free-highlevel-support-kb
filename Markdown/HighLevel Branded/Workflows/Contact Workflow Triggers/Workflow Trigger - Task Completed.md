**Date Updated:** 2025-02-26T19:36:33.000Z

Managing tasks efficiently is key to maintaining smooth business operations. The Task Completed Workflow Trigger in HighLevel helps automate follow-ups and next steps as soon as a task is marked as completed. This guide will walk you through its functionality, benefits, and step-by-step configuration.

---

**TABLE OF CONTENTS**

* [What is the Task Completed Workflow Trigger?](#What-is-the-Task-Completed-Workflow-Trigger?)
* [Key Benefits of the Task Completed Workflow Trigger](#Key-Benefits-of-the-Task-Completed-Workflow-Trigger)
* [Configuring the Task Completed Workflow Trigger](#Configuring-the-Task-Completed-Workflow-Trigger)
* [Frequently Asked Questions](#Frequently-Asked-Questions)

---

# **What is the Task Completed Workflow Trigger?**

  
The Task Completed Workflow Trigger is designed to automatically execute actions in a workflow whenever a task is marked as completed in the CRM. This ensures seamless automation of follow-ups, notifications, and process advancements, reducing manual effort and enhancing team productivity.

---

## **Key Benefits of the Task Completed Workflow Trigger**

  
* **Automated Task Follow-Ups:** Ensures the next steps happen automatically after a task is completed.

  
* **Enhanced Team Collaboration:** Notifies assigned team members or other stakeholders about completed tasks.

  
* **Process Efficiency:** Moves tasks forward in workflows without requiring manual intervention.

  
* **User-Specific Automation:** Allows workflows to trigger based on the Assigned User filter.

  
* **Accurate Task Tracking:** Keeps CRM data up to date with completed tasks.

---

## **Configuring the Task Completed Workflow Trigger**

  
### **Accessing the Workflow Builder**

  
Start by navigating to the **Automation** section in your HighLevel dashboard. If you’re setting up a new workflow, click **\+ Create Workflow** and then select **\+ Start from Scratch**. Alternatively, you can modify an existing workflow to include the Task Completed trigger.

  
![](https://s3.amazonaws.com/cdn.freshdesk.com/data/helpdesk/attachments/production/155042034342/original/g5qw4injNkpmSYRFxrfnNtwlm9iHugRvMg.png?1740148687)  

  
### **Adding the Task Completed Trigger**

  
To add the Task Completed trigger to your workflow, Click on **\+ Add New Trigger** and search for **Task Completed** in the available trigger list. Once found, select it to ensure the workflow initiates automatically whenever a task is marked as completed.

  
![](https://s3.amazonaws.com/cdn.freshdesk.com/data/helpdesk/attachments/production/155042034384/original/2vOEXiiM3_red78xpkaDpM34_hOSqB1HYA.png?1740148710)  

  
### **Applying the Assigned User Filter**

  
To refine automation and ensure tasks are completed by specific team members, you can apply the Assigned User filter. This filter allows you to trigger workflows based on who completed the task.

  
After selecting the Task Completed trigger, choose the Assigned User filter and set the appropriate operator:

* **Is:** The workflow triggers only when the selected user completes the task.
* **Is Empty:** The workflow triggers if the task has no assigned user.
* **Is Not:** The workflow triggers for all users except the selected one.
* **Is Not Empty:** The workflow triggers when a task has an assigned user.

  
Once you choose an operator, the next dropdown will display all available CRM users, allowing you to select specific team members. If no filter is applied, the workflow will trigger whenever any user completes a task, ensuring flexibility based on your business needs.

  
![](https://s3.amazonaws.com/cdn.freshdesk.com/data/helpdesk/attachments/production/155042034421/original/RgmJIhW_ih4ZdJ9coSzQA4KPjKhiTu2o3Q.png?1740148745)  

  
### **Define Workflow Actions**

  
After setting up the trigger, add workflow actions to automate the next steps. 

  
Examples include:

* **Send Notification:** Notify team members when a task is completed.
* **Update CRM Record:** Modify contact or opportunity details after task completion.
* **Move Opportunity to the Next Stage:** If the task is linked to a sales opportunity, advance it to the next stage.
* **Trigger Another Workflow:** Activate another workflow based on task completion.

If you are looking for a detailed guide about using a specific workflow action, you can refer to the respective article in our Knowledge Base library.

---

## **Frequently Asked Questions**

  
**Q: Can I trigger workflows only for tasks completed by specific users?**

Yes, use the Assigned User filter and select a team member using the “Is” operator.
  
  
**Q: What happens if a task has no assigned user?**

You can use the “Is Empty” filter operator to trigger workflows only for unassigned tasks.
  
  
**Q: Can this trigger send automated notifications?**

The trigger itself does not send notifications, but you can add a Send Notification action to alert team members.
  
  
**Q: Can this workflow update an opportunity after task completion?**

Yes, you can set an action to update the opportunity pipeline or status once a task is marked as completed.
  
  
**Q: How do I check if the workflow is working properly?**

You can track execution in the Workflow Execution Log to see if the trigger fires correctly when a task is completed.

This version now includes the correct filter operators and team member selection.