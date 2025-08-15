**Date Updated:** 2024-12-20T06:17:08.000Z

The Custom Webhook Action enables real-time data exchange between your CRM and third-party services. It allows tailored requests with various HTTP methods, authorization, headers, and query parameters. This user-friendly tool ensures efficient and accurate workflows while considering API responses and server limitations.  
  
  
**Agencies on** **Any Plan** ($97, $970, $297, $2970, $497, $4970) can access LC Premium Triggers & Actions.  
  
- Once Premium Actions & Triggers are enabled via the Agency settings, EXISTING and New Sub-Accounts will have **100 free executions**.  
   
- For agencies to avoid accruing execution costs for EXISTING Sub-Accounts, rebilling will need to be enabled **manually** for each Sub-Account within the Agency view ([more info](https://help.gohighlevel.com/support/solutions/articles/48001231559-how-to-enable-lc-premium-triggers-actions-for-workflows#How-to-turn-on-re-billing-for-my-clients?:~:text=Re%2Dbilling%20the%20costs%20to%20your%20clients%20and%20making%20a%20profit)).   
  
- If premium actions are **enabled** on the SaaS Configurator, new Sub-Accounts generated will automatically be enrolled in LC Premium Actions & Triggers, **no further** action is required by the agency.
  
  
**TABLE OF CONTENTS**

* [What is the Custom Webhook Action?](#What-is-the-Custom-Webhook-Action?)
* [Who is this feature useful for?](#Who-is-this-feature-useful-for?)
* [Key Benefits](#Key-Benefits)
* [How To Setup Custom Webhook](#How-To-Setup-Custom-Webhook)
* [Step 1: Fill Url](#Step-1%3A%C2%A0Fill-Url)
* [Step 2: Select a Method](#Step-2%3A%C2%A0Select-a-Method)
* [Step 3: Select Authorization Method](#Step-3%3A%C2%A0Select-Authorization-Method)
* [Step 4: Headers & Query Parameters](#Step-4%3A%C2%A0Headers-&-Query-Parameters)
* [Step 5: Configure the data to be sent in the Custom Webhook](#Step-5%3A%C2%A0Configure-the-data-to-be-sent-in-the-Custom-Webhook)
* [Troubleshooting](#Troubleshooting)

---

# **What is the Custom Webhook Action?**

  
The Custom Webhook - LC Premium Action is a powerful and flexible feature that enables real-time communication between your CRM system and third-party services. It allows you to configure and send custom data requests to specified URLs using different HTTP and authorization methods. 

  
This feature also supports adding headers, query parameters, and mapping custom values to create a tailored request structure that meets your needs. With autocomplete suggestions and user-friendly interfaces, the Custom Webhook streamlines data exchange and ensures accuracy in your workflows. However, it is crucial to consider API response success and server limitations when using this feature to prevent errors and disruptions in workflow execution.

  
## **Who is this feature useful for?**

  
This feature is helpful for businesses and individuals who need to integrate their CRM systems with third-party services for seamless data exchange, automation, and enhanced functionality. It is particularly useful for marketers, developers, and IT professionals who want to streamline workflows, improve data consistency, and manage processes more efficiently across various platforms.

  
## **Key Benefits**

  
* **Accurate integration:** Creates communication between your CRM system and third-party services, replacing manual error-prone data entry. Autocomplete suggests data mapping.
* **Flexibility:** Supports various HTTP methods, authorization methods, headers, and query parameters, allowing you to create custom requests that suit your needs.
* **Real-time updates:** Facilitates real-time notifications and updates, enhancing responsiveness and decision-making.
* **Scalability:** Adaptable to various industries and requires no changes as you scale operations.

  
---

## **How To Setup Custom Webhook**

  
### **Step 1:** Fill Url

  
You have the ability to send data requests to any URL of your choice without the need for coding or server operation.

  
![](https://s3.amazonaws.com/cdn.freshdesk.com/data/helpdesk/attachments/production/48294091111/original/EDBmiD3CByaY9AzWrugDV5p_sgu4UjDWhg.png?1682327841)

  
### **Step 2:** Select a Method

  
You can choose any HTTP method that suits your needs, such as POST, GET, DELETE, or PUT.

  
![](https://s3.amazonaws.com/cdn.freshdesk.com/data/helpdesk/attachments/production/48294091211/original/fn4VdG-17mzKyBYaCKVsdkdCo_VMZC7tmg.gif?1682327875)

  
### **Step 3:** Select Authorization Method

  
We support various types of authorization methods, allowing you to choose the one that suits your needs when accessing the webhook. 

  
![](https://s3.amazonaws.com/cdn.freshdesk.com/data/helpdesk/attachments/production/48294091321/original/KDoCu7K61OSjQcvg9r4zWGOgjFAD1idHLg.gif?1682327914)

  
### **Step 4:** Headers & Query Parameters

  
In addition to sending a request body, our system allows you to include headers and query parameters when sending requests to a webhook.

  
Headers can be used to provide additional information about the request, such as authentication credentials, content type, and cache control. 

  
Query parameters, conversely, can be used to pass parameters to the webhook endpoint, allowing you to filter or modify the response data you receive.

  
![](https://s3.amazonaws.com/cdn.freshdesk.com/data/helpdesk/attachments/production/48294091453/original/NTQRsd_lJ9jCRHBNB3U3Q5s4jhVcucDt6A.gif?1682327951)

  
### **Step 5:** Configure the data to be sent in the Custom Webhook

  
The Custom Webhook premium feature allows you to map custom values in any structure that suits your requirements. Our user-friendly textbox provides autocomplete suggestions for all custom values, including inbound webhook variables.

  
This feature simplifies the mapping process and saves time by suggesting potential values that match your input. Additionally, it helps ensure accuracy and consistency in your data mapping.

  
![](https://s3.amazonaws.com/cdn.freshdesk.com/data/helpdesk/attachments/production/48294091557/original/Sw2g0QozPRAO007VglNJeG3jDYJRHUwiaw.gif?1682327991)

  
## **Troubleshooting**

  
Successful execution of the Custom Webhook Action depends on the successful response of the referenced API. Therefore, if errors are sent back, those will reflect on the Contact's Workflow execution and cause the action to be Failed (and then skipped) or Retry with exponential backoffs. 

  
Make sure that the receiving server can handle the number of Executions that you are targeting, or else you might end up with errors due to limits being reached. The Custom Webhook Action will get fired as soon as the Contact reaches the step, so make sure to add Contacts into the Workflow with the receiving server's limits in mind.

  
### 

  