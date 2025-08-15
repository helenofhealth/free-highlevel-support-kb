**Date Updated:** 2025-04-09T02:45:22.000Z

**TABLE OF CONTENTS**

* [Overview](#Overview)
* [Action Name](#Action-Name)
* [Action Description](#Action-Description)
* [Action Details](#Action-Details)
* [Example](#Example)

##   

## Overview

  
The Custom Webhook Action allows you to integrate your with external systems by sending real-time data via HTTP POST, GET, PUT and Delete methods. This action enables seamless automation, data exchange, and interaction with third-party services, APIs, and custom applications without requiring any coding.

  
## Action Name

Custom webhook

  
## Action Description

The Custom Webhook Action enables users to send HTTP requests to specified URLs, integrating with external services for automated data exchange. This action supports multiple HTTP methods (POST, GET, PUT, DELETE), customizable headers, query parameters, and authentication options to match the needs of any third-party service.

Supported Features:

* **HTTP Methods:** POST, GET, PUT, DELETE
* **Custom Headers & Query Parameters:** Pass authentication, content-type, or other necessary data
* **Authorization Methods:**Basic Auth, Bearer token, API key and No auth.  
   * Basic Auth requires Username and Password  
   * Bearer token requires Token of the platform  
   * API key requires a key-value pair of the key name and its value ie the API key.
* **Data Mapping:** Autocomplete suggestions to map custom values like contact info, lead status, and more

  
## Action Details

  
#### Step-by-Step Guide

1. **Choose the Action Type:**  
   * Select "Custom Webhook" from the list of available actions in the workflow builder.
2. **Name Your Action:**  
   * Enter a descriptive name, such as "Send Data to External API."
3. **Enter the Webhook URL:**  
   * Provide the URL of the external system’s endpoint where the data should be sent (e.g., a CRM, payment gateway, or custom API).
4. **Select HTTP Method:**  
   * Choose from POST, GET, PUT, or DELETE depending on the type of data operation required by the external service.
5. **Select Authorization Method (Optional):**  
   * Choose the necessary authorization method such as API keys, Bearer Tokens, or Basic Auth to ensure secure communication with the external service.
6. **Configure Headers & Query Parameters (Optional):**  
   * Add any required headers like `Authorization: Bearer <API_KEY>` or content-type headers to define the data format (`Content-Type: application/json`).  
   * Use query parameters to pass additional information, filter data, or adjust the external API’s response.
7. **Map Data:**  
   * Insert relevant data (e.g., contact name, email, phone number) into the request body. You can structure the payload in JSON or another format required by the external system. Example Payload:

```javascript
{ "first_name": "{{contact.first_name}}", "last_name": "{{contact.last_name}}", "email": "{{contact.email}}", "phone": "{{contact.phone}}" }
```

JavaScript

1. **Save and Activate the Workflow:**  
   * Once set up, activate the workflow. The webhook will trigger and send data in real time based on the workflow conditions.

  
![](https://s3.amazonaws.com/cdn.freshdesk.com/data/helpdesk/attachments/production/155032302044/original/PFAnKNR1PW1eEsV7LkiUV0Fuko7i8XMLjw.png?1725530767)

  
## Example

  
**Scenario:** A business wants to send contact information to an external CRM whenever a new lead is created in your system.

1. **Create Workflow Trigger:**  
   * Set up a workflow trigger for when a new lead is created.
2. **Add Custom Webhook Action:**  
   * Choose "Custom Webhook" and name it "Send Lead Data to CRM."  
   * Webhook URL: `https://api.externaltestcrm.com/leads/create`  
   * HTTP Method: POST  
   * Payload  
   `{  
     "first_name": "{{contact.first_name}}",  
     "last_name": "{{contact.last_name}}",  
     "email": "{{contact.email}}",  
     "phone": "{{contact.phone}}"  
   }  
   `  
   * Headers: Add an API key to authenticate the request  
         * `Authorization: Bearer xyz123`  
         * `Content-Type: application/json`
3. **Test the Webhook:**  
   * Test using a tool like Webhook.site or Postman to confirm the data is correctly sent and received.
4. **Save and Activate:**  
   * Once activated, the webhook will automatically send lead data to the CRM whenever a new lead is created.

**Outcome:** Every new lead is synced with the external CRM, improving automation and reducing manual data entry.
  
  
## Frequently Asked Questions

  
**Q: My third-party service requires a static IP address to whitelist for webhooks. What should I do?**

  
**A:** The platform does not provide a static IP address or range for whitelisting. This is because the system operates on a dynamic, real-time cloud infrastructure, which is the standard for modern, scalable services.

  
The correct and more secure method is to authenticate using a secret key or token sent in the request's header. 

  
You should take one of the following two approaches based on your third-party provider's requirements:

  
**1\. If Your Provider Uses a Standard Authentication Method:**

If your provider uses a common method like a Bearer Token or a standard API Key, you can use the built-in authorization options.

* In the **AUTHORIZATION** dropdown, select the appropriate method (e.g., "Bearer Token" or "API Key").
* Enter the credentials provided by the third-party service.
  
  
**2\. If Your Provider Uses a Custom Header for Authentication:**

If the third-party provider requires a unique key and value in the header for verification, follow these steps:

* In the **AUTHORIZATION** dropdown, select **None**.
* Navigate to the **HEADERS** section below.
* Click **Add item** and enter the custom **Key** and **Value** that the third-party service has provided to you.

  
You should inform your third-party provider that your system uses modern, header-based authentication and ask them for the necessary credentials to send with each request.
  
  