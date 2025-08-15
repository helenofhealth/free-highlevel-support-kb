**Date Updated:** 2023-05-05T19:10:48.000Z

The Eliza Agent Platform is a messaging platform designed to help agencies effectively manage and convert leads into customers. With its three key features - lead answering, scalable lead nurturing, and streamlined booking flow - Eliza is the perfect solution for agencies that want to provide excellent customer service and improve their lead conversion rates.
  
  
#### **Covered in this Article**

#### [**What is the Eliza Agent Platform?**](#What-is-the-Eliza-Agent-Platform?)

#### [**FAQs - Eliza Agent Platform**](#FAQs---Eliza-Agent-Platform)

* #### [1\. How does the custom value user? Name work in Eliza Agent Platform?](#1.-How-does-the-custom-value-user?-Name-work-in-Eliza-Agent-Platform?)
* #### [2\. How to bring contacts into Eliza without an inbound message or the one who made an inbound call?](#2.-How-to-bring-contacts-into-Eliza-without-an-inbound-message-or-the-one-who-made-an-inbound-call?)
* #### [3\. I see conversations on GHL, but they are not coming into Eliza.](#3.-I-see-conversations-on-GHL,-but-they-are-not-coming-into-Eliza.)
* #### [4\. How to update the API key on the Eliza Agent Platform?](#4.-How-to-update-the-API-key-on-the-Eliza-Agent-Platform?)
* #### [5\. How to make blind and warm transfers in calls?](#5.-How-to-make-blind-and-warm-transfers-in-calls?)  
   * #### [Blind Transfer](#Blind-Transfer)  
   * #### [Warm Transfer](#Warm-Transfer)  
   * #### [Troubleshooting:](#Troubleshooting%3A)
* #### [6\. When an appointment is created for a contact, the contact is not removed from the chat queue. Do I need to do anything special to make them be removed (as far as tags go or anything?)](#6.-When-an-appointment-is-created-for-a-contact,-the-contact-is-not-removed-from-the-chat-queue.-Do-I-need-to-do-anything-special-to-make-them-be-removed-%28as-far-as-tags-go-or-anything?%29)
* #### [7\. I can't see the Eliza Service tab on GHL in sub-account> Settings.](#7.-I-can't-see-the-Eliza-Service-tab-on-GHL-in-sub-account%3E-Settings.)

  
**Related Articles**  
[Eliza Agent Platform Settings within the CRM](https://help.gohighlevel.com/support/solutions/articles/48001236605-eliza-agent-platform-settings-within-the-crm)

[Eliza Agent Platform Settings](https://help.gohighlevel.com/support/solutions/articles/48001236575-eliza-agent-platform-settings)

[Eliza Agent Platform Search Tools](https://help.gohighlevel.com/support/solutions/articles/48001236599-eliza-agent-platform-search-tools)

[Eliza Agent Platform Dashboard](https://help.gohighlevel.com/support/solutions/articles/48001236604-eliza-agent-platform-dashboard)

[Eliza Agent Platform Conversations](https://help.gohighlevel.com/support/solutions/articles/48001236598-eliza-agent-platform-conversations)

  
---

## **What is the Eliza Agent Platform?**

  
The Eliza Agent Platform is a messaging platform to help Agencies boost conversions by nurturing their leads into customers for them. One of the primary features of Eliza is its ability to answer leads for clients quickly. This helps agencies respond to customer inquiries promptly and efficiently, ensuring that leads are not lost due to slow response times.to answer leads for clients quickly

  
Eliza also allows agencies to create a scalable process for nurturing leads. This feature helps agencies develop a system that can handle large volumes of leads and efficiently manage converting those leads into customers.

  
Finally, the Eliza Agent Platform helps to streamline the booking flow. By providing a customizable FAQ setup and Agent Configuration, Eliza makes it easy for agents to manage the booking process and respond to customer inquiries in real time.

  
It is important to note that the Eliza Agent Platform does not offer conversation bots. However, this feature is available in the platform's PRO plan if an agency is looking for a conversational appointment booking bot, this feature is available in the platform's PRO plan.

  
Overall, the Eliza Agent Platform is an ideal solution for agencies that want to offer a human rollover system to their customer base within their Agency Account. By providing a scalable and efficient process for managing leads, Eliza helps agencies to work smarter, not more complex, and improve their lead conversion rates.

  
**You can purchase the Eliza Agent Platform service [here.](https://mp.gohighlevel.com/eliza-agent-platform)** 

---

## **FAQs - Eliza Agent Platform**

  
### **1\. How does the custom value user? Name work in Eliza Agent Platform?**

* When a user is assigned to a contact, and if the user. Name is used in workflow or Eliza; it will substitute the assigned user. However, when the same template is used from the conversations screen of the main app, then the logged-in user's name will be taken irrespective of whether there is an assigned user.name
* When there is no assigned user to the contact, workflows and Eliza will substitute the user. name with a blank.
* Thus, if you want to give a valid value to the user. name in Eliza, then the contact should be assigned to someone on the GHL side for Eliza ( and workflows) to pick it up., name
* Sometimes, the +Assigned To link may not be visible on Eliza. The fix is to refresh the API key on the main app and use the new one for this location.

  
### **2\. How to bring contacts into Eliza without an inbound message or the one who made an inbound call?**

In cases where the contact does not send inbound messages or makes only inbound calls, the contact does not automatically come into Eliza. In those cases, use Send to Eliza action from the workflows and send them to Eliza.

  
**Send to Eliza Workflow action.**

Configure the Send to Eliza workflow action for the qualifying contacts and let the platform take care of it automatically for you. 

  
If a Send to Eliza tag is configured to be assigned to the leads coming into Eliza, that tag will also be assigned before the contact is sent over. This tag assignment is not mandatory for this action to work.

![](https://s3.amazonaws.com/cdn.freshdesk.com/data/helpdesk/attachments/production/48290277854/original/zmH2Xs3HSvlF4NySnMbkMbaZ0AFDNyF44A.png?1680197106)
  
  
**On the Eliza Agent Platform**

  
When the contact is received in Eliza via Send to Eliza workflow action, it will have a timer icon, as shown below. ![](https://s3.amazonaws.com/cdn.freshdesk.com/data/helpdesk/attachments/production/48290278728/original/OwTeg-3dBKAlY8mXy9-7i60Sj3Grm8Gc2A.png?1680197517)

If you want to specifically nurture only those contacts sent by the "Send to Eliza" workflow action, you can also filter only for those conversations. Choose the "Sent to Eliza" option and click "Go" to see only those messages sent by workflow action.![](https://s3.amazonaws.com/cdn.freshdesk.com/data/helpdesk/attachments/production/48290280129/original/TPbfeD5h2OG5hlWzjYabXe5FPm6PPE28uA.png?1680198050)
  
  
### **3\. I see conversations on GHL, but they are not coming into Eliza.**

Only inbound messages will come into Eliza automatically.

* Inbound calls are not pushed into Eliza yet as it is not supported. But we are working on inbound call management and will be available sometime during H1, 2022.
* If you want to push these inbound calls into Eliza and nurture the leads, use the Send to Eliza action in workflows. Refer to FAQ#2 for more details.

  
If you want to analyze the audit log of the conversation history in Eliza, go to Search > contact, choose the contact, and click the Audit log button. If this contact ever got into Eliza, it will show the audit log of the conversation history.

  
### **4\. How to update the API key on the Eliza Agent Platform?**

Please follow [this link](https://help.gohighlevel.com/support/solutions/articles/48001205369-how-to-update-your-api-keys). 
  
  
### **5\. How to make blind and warm transfers in calls?**

#### **Blind Transfer**

  
A Blind Transfer is when you transfer the caller to another extension or ring group (queue) without waiting for the target agent to pick up first. It is an immediate, unannounced call transfer to the destination number.

  
Start the outbound call to the lead by clicking the phone icon.

![](https://s3.amazonaws.com/cdn.freshdesk.com/data/helpdesk/attachments/production/48290282661/original/BGEYxIy7PQMIvs-U_zTE07nO9ImgCzNvrA.png?1680199220)

You will see the note at the top of the conversation page when the call is in progress, as shown below.![](https://s3.amazonaws.com/cdn.freshdesk.com/data/helpdesk/attachments/production/48290282879/original/cl4bI_W7IFgKIEzTOg3rPeY8pLBvBN9vqw.png?1680199335)
  
  
Click the down arrow next to the dialer icon on the popup to make the blind transfer.

  
Click on **Blind transfer.**![](https://s3.amazonaws.com/cdn.freshdesk.com/data/helpdesk/attachments/production/48290283562/original/cGw3zjRegHF2G_leIl3MVV1bssij5mx10A.png?1680199594)

Choose the GHL team member from the list shown. 

  
Only those numbers already part of the GHL team Section can be transferred. Select the team member to whom this call should be transferred, and click "Call & Disconnect."
  
  
If you want to add a new member, login into GHL and create a new team member with their phone number. 

If you want another Eliza agent to call this customer, transfer the conversation to that agent via Seach > Contacts. We will soon be able to transfer the call to another Eliza Agent directly.![](https://s3.amazonaws.com/cdn.freshdesk.com/data/helpdesk/attachments/production/48290284237/original/90SL7IkChGM-QR2vnFWhM0qh1djmdz51RQ.png?1680199792)
  
  
#### **Warm Transfer**

  
A warm call transfer means that the receptionist will speak with the appropriate agent before they send the call to them. The extension the caller requested is informed of the incoming call transfer. Typically, the caller will be put on hold while the call center operator dials the desired extension.
  
  
Make an outbound call to the contact.![](https://s3.amazonaws.com/cdn.freshdesk.com/data/helpdesk/attachments/production/48290284464/original/KP91iRzUaj4p-o582uM6Re9ZS5cOTeGfEw.png?1680199872)

From the popup that appears at the top of the page, Choose "Warm Transfer."![](https://s3.amazonaws.com/cdn.freshdesk.com/data/helpdesk/attachments/production/48290285574/original/M49LxiFS7NuAaVsnRlhhIL9wcFIYnK_LJg.png?1680200267)

Choose the number to warm transfer this call, then click **"Call and Hold."![](https://s3.amazonaws.com/cdn.freshdesk.com/data/helpdesk/attachments/production/48290285746/original/AZ-QQpRwFtJF7KtohqfZRWbxisoWAkk5bQ.png?1680200344)**

  
The system will wait for agent 2 to pick up the call.

  
![](https://s3.amazonaws.com/cdn.freshdesk.com/data/helpdesk/attachments/production/48290285805/original/mFvN2-naURLU1_ygBnHeI5NUIOiLf0YoGA.png?1680200365)
  
  
Once agent 2 attends the call, click "Patch Call" to put all three numbers in a conference. 

  
Press the red color "Drop Off" button to disconnect from the conference. This action will let the contact and agent 2 continue their conversation.![](https://s3.amazonaws.com/cdn.freshdesk.com/data/helpdesk/attachments/production/48290285949/original/2fANLYcMpyBemclwowS5O4gGxcd8-lM5sQ.png?1680200423)
  
  
#### **Troubleshooting**:

  
If the system becomes inconsistent, ensure the browser can access the microphone and refresh the page to ensure the connection with Twilio goes through correctly.

![](https://s3.amazonaws.com/cdn.freshdesk.com/data/helpdesk/attachments/production/48290286221/original/XXfs03-cg7pATtpKn67NwpvO-FJiRUx7JA.png?1680200540)

![](https://s3.amazonaws.com/cdn.freshdesk.com/data/helpdesk/attachments/production/48290286374/original/OEyUVqeTWhTUKTQqfzMs4ZDhVd56MNlTnA.png?1680200606)

  
### **6\. When an appointment is created for a contact, the contact is not removed from the chat queue. Do I need to do anything special to make them be removed (as far as tags go or anything?)**

The system will not know if booking an appointment ends the conversation. So it will keep it open. Agents can close the conversation by clicking "End Chat." If you don't have any further dispositions to be assigned, you can choose the "Close without a disposition" button and close the conversation.."

###   

### **7\. I can't see the Eliza Service tab on GHL in sub account> Settings.**

![](https://s3.amazonaws.com/cdn.freshdesk.com/data/helpdesk/attachments/production/48290287736/original/Z4U7d0EG-pjPhhVNMxrMJslWHQOkPr3hvA.png?1680201231)

Please check for the following conditions.

  
* If the location is added to your account on Eliza Agent Platform
* The email address of the user who is expected to have access to the Location settings > Eliza Service tab should be added as a location admin or location user for that location
* That same email address should have Eliza Service permission enabled, so they can edit the FAQs and configure Eliza bypass tag and the Send to Eliza tag on Location Settings > Eliza Service tab.

  