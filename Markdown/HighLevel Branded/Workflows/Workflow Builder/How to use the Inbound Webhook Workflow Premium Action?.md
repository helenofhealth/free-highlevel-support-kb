**Date Updated:** 2025-02-28T02:46:19.000Z
  
  
Inbound Webhooks enable seamless CRM integration by allowing external systems to automatically send data using various HTTP request methods like GET, POST, and PUT. This real-time data transfer capability enhances CRM functionality and streamlines workflows, facilitating efficient communication and collaboration across various platforms and tools.

  
- **Agencies on** **Any Plan** ($97, $970, $297, $2970, $497, $4970) can access LC Premium Triggers & Actions.  
  
- Once Premium Actions & Triggers are enabled via the Agency settings, EXISTING and New Sub-Accounts will have **100 free executions**.  
   
- For agencies to avoid accruing execution costs for EXISTING Sub-Accounts, rebilling will need to be enabled **manually** for each Sub-Account within the Agency view ([more info](https://help.gohighlevel.com/support/solutions/articles/48001231559-how-to-enable-lc-premium-triggers-actions-for-workflows#How-to-turn-on-re-billing-for-my-clients?:~:text=Re%2Dbilling%20the%20costs%20to%20your%20clients%20and%20making%20a%20profit)).   
  
- If premium actions are **enabled** on the SaaS Configurator, new Sub-Accounts generated will automatically be enrolled in LC Premium Actions & Triggers, **no further** action is required by the agency.
  
  
#### **Covered in this Article**

#### [**What is an Inbound Webhook?**](#What-is-an-Inbound-Webhook?)

#### [What are some excellent usage cases for this?](#What-are-some-excellent-usage-cases-for-this?)

####   
[**How to use the Inbound Webhook Workflow Trigger?**](#How-to-use-the-Inbound-Webhook-Workflow-Trigger?)

#### [Step 1](#Step-1)

#### [Step 2](#Step-2)

#### [Step 3](#Step-3)

#### [In your communication Actions:](#In-your-communication-Actions%3A)

#### [In If/Else Actions:](#In-If/Else-Actions%3A)

#### [Important points to be considered:](#Important-points-to-be-considered%3A)

---

## **What is an Inbound Webhook?**

An Inbound Webhook is a robust feature that facilitates the automatic data transfer from external systems to your CRM, improving integration and interoperability. When an event occurs in an external system, an HTTP request (POST, GET, or PUT) is sent to a specific URL linked to a trigger within your CRM, initiating a workflow. This real-time data transfer capability enhances your CRM's functionality and streamlines workflows across various platforms and tools.

  
By leveraging Inbound Webhooks, businesses can automate processes, reduce manual tasks, and minimize human error, increasing efficiency and productivity. Furthermore, it enables better collaboration between teams, as critical data is readily available and synchronized between different systems. This seamless integration ultimately improves decision-making, customer satisfaction, and business performance.

  
### **What are some excellent usage cases for this?**

  
Inbound Webhooks can be used in various scenarios to enhance CRM functionality and automate workflows. Here are a few practical usage cases with examples:

  
**eCommerce Order Integration:**

Suppose you have an online store and want to update your CRM with new order information when a customer orders. You can set up an Inbound Webhook in your CRM to receive data from your eCommerce platform whenever a new order is created.

Example: Your eCommerce platform sends an HTTP POST request to the webhook URL with order details such as customer name, email, phone number, and order value. Your CRM then creates or updates the customer's contact information and adds the order details to their record.

  
**Customer Support Ticketing System Integration:**

Your company may use a separate support ticketing system to handle customer issues. When a customer creates a support ticket, you can use an Inbound Webhook to send the ticket details to your CRM, ensuring the support team has all the necessary information.

Example: Your support ticketing system sends an HTTP POST request to the webhook URL with the ticket details, including customer email, ticket title, and description. Your CRM then associates the ticket with the corresponding customer record, allowing your support team to access the ticket information directly from the CRM.

  
**Event Registration Integration:**

If you host events and use an event registration platform, you can use an Inbound Webhook to send attendee registration information to your CRM.

Example: Your event registration platform sends an HTTP POST request to the webhook URL with attendee information such as name, email, phone number, and event name. Your CRM then creates or updates the attendee's contact information and adds the event registration details to their record, allowing your event team to manage and communicate with attendees effectively.

  
**Lead Capture from Web Forms:**

Inbound Webhooks can capture leads from web forms on your website or landing pages and send the data to your CRM.

Example: When a visitor submits a form on your website, your web form sends an HTTP POST request to the webhook URL with the lead's information, such as name, email, and phone number. Your CRM then creates a new lead or updates an existing contact, allowing your sales team to follow up with the lead promptly.

  
These are just a few examples of how Inbound Webhooks can automate workflows, streamline processes, and enhance CRM functionality in different business scenarios.
  
  
## **How to use the Inbound Webhook Workflow Trigger?**

Briefly, bring your data to the system in 3 simple steps using the Inbound Webhook Trigger.

  
![](https://s3.amazonaws.com/cdn.freshdesk.com/data/helpdesk/attachments/production/48296396414/original/5xlRF80hbq19hXS2IeQjhZ5GlPK6xGxPLQ.png?1683557063)

  
#### **Step 1**

Retrieve the webhook URL and use it in your application or system. Next, send the data to the webhook URL using the appropriate HTTP request method (POST, GET, or PUT) and click the "Test Trigger" button.  
  
![](https://s3.amazonaws.com/cdn.freshdesk.com/data/helpdesk/attachments/production/48296396436/original/IlVVYc7eyGT9KdCkdq9wlbT68qjQH71BzA.jpeg?1683557066)
  
  
#### **Step 2**

Choose the data received from your application or system using the supported HTTP request method (POST, GET, or PUT) and save it as sample data for future reference. Click on "Load More" to view additional recent data. Once you've selected the desired data, save the trigger.

  
In this step, you can save the data reference for custom variables, which can be treated similarly to other contact custom fields or Location Custom Variables.

  
The next step and examples below provide more information on utilizing this reference.

  
Step 2.1: Send a supported HTTP request (POST, GET, or PUT) to the copied webhook URL and copy the ID in the response.
  
  
![](https://s3.amazonaws.com/cdn.freshdesk.com/data/helpdesk/attachments/production/48296396447/original/HBssN92Dcn7RELV0WfeiQvdzyYoVWnZesA.jpeg?1683557067)
  
  
Step 2.2: Copy the unique ID obtained from the supported HTTP request (POST, GET, or PUT) and use it to search for the relevant mapping reference within your webhook trigger.

  
Please note that the most recent request will always be at the top of the list.

  
![](https://s3.amazonaws.com/cdn.freshdesk.com/data/helpdesk/attachments/production/48296396689/original/1GOfBLW8pVhtm0-4jBOU-djexnqbxJUQhg.gif?1683557143)

  
Step 2.3: Select the correct reference and verify the body.  
  
![](https://s3.amazonaws.com/cdn.freshdesk.com/data/helpdesk/attachments/production/48296396424/original/jE6MPEf9WpVPFFQ0ahHfacR6JsSdqJRmyQ.png?1683557064)

###   

#### **Step 3**

You will be directed to the "Create Update Contact" action after saving the trigger. "Create Update contact From there, you can select the necessary fields and map the incoming data you received from the trigger. Please note that to create a new contact or map data to an existing one, you must provide either an email or phone field. If your trigger data is not carrying email or phone you can remove this action from workflow and workflow will continue to execute contactless.  
  
  
![](https://s3.amazonaws.com/cdn.freshdesk.com/data/helpdesk/attachments/production/48296396430/original/dLt6e4aBJ-RSHELvUaJx6MD8J6i5jOaOKw.jpeg?1683557066)

  
---
  
  
By completing the above steps, you can now use the data you received within the workflow as custom values in email, sms, if/else, etc.  
  
  
![](https://s3.amazonaws.com/cdn.freshdesk.com/data/helpdesk/attachments/production/48296396440/original/WDyICG5QVeEo1X5iv-AAmEjLhl6HhJKn1Q.png?1683557067)
  
  
---

**Example:**

  
The custom values of Inbound Webhook can be utilized in all of the actions within your workflow. Some examples of how to do this are provided below.
  
  
### **In your communication Actions:**  
  
![](https://s3.amazonaws.com/cdn.freshdesk.com/data/helpdesk/attachments/production/48296396872/original/Y_f4vN7W6D0Af8UpHCCStiQq-BLwJiMb0g.gif?1683557198)
  
  
#### **In If/Else Actions:**

![](https://s3.amazonaws.com/cdn.freshdesk.com/data/helpdesk/attachments/production/48296396946/original/HMKEQnrIHJvwPHaAiEUA2z2sjFgjgBELvA.gif?1683557230)

  
As shown above, you can use the values from the Inbound Webhook inside all other actions as you see fit.
  
  
## **Can workflow execute without contact?**

* Workflow can run contactless without any Contact data dependency so you can send any payload data via Inbound Webhook Triggers and use it in workflow.
* You can proceed without contact and use actions that are not dependent on contact information. Custom Webhook, Google Sheet, Slack, ChatGPT and all Internal Tools can be executed without contact.
* If necessary, you can use the Create/Update or Find Contact actions to retrieve the contact data to the workflow.  
    
**Example:**
* Send order data via inbound webhook and add the order information to google sheet, use if/else to categorize based on order value and send a slack notification.
* Retrieve the contact with Contact ID using Find contact action

---

  
#### Important points to be considered:

  
* Always send the request using a supported method (POST, GET, or PUT) when interacting with the webhook.
* Ensure the data is sent as a JSON object, the only supported data format.
* To compile correctly, keys must be a single string without space separations; consider using CamelCase or snake\_case instead of separating key names with spaces.
* Providing an Email or Phone number in the payload is mandatory, as the workflow requires contact information. An Email or Phone is required to Find or Create the Contact.
* Arrays are not supported in custom values. You can send them in the request but cannot use them inside actions.
* If your data structure changes, re-select the Mapping Reference inside the Inbound Webhook Trigger setup to address those fields in other actions correctly.
* If your Inbound Webhook Trigger URL gets compromised or leaked and you want to prevent unwanted requests, Delete the existing Inbound Webhook Trigger and Add a New Inbound Webhook Trigger. A new URL with a different ending ID will be generated; update your integrations to match the new URL. Once saved, incoming requests from the old URL won't enter your workflow; only requests from the new URL will.

  