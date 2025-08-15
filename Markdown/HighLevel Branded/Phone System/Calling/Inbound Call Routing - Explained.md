**Date Updated:** 2024-10-21T13:47:23.000Z

  
**TABLE OF CONTENTS**

* [Incoming Call to a Phone number](#Incoming-Call-to-a-Phone-number)
* [FAQs:](#FAQs%3A)  
   * [1\. How would we know which Phone number the contact call if we have more than one Phone number?](#1.-How-would-we-know-which-Phone-number-the-contact-call-if-we-have-more-than-one-Phone-number?)  
   * [2\. How to check if the Phone number is assigned to a user?](#2.-How-to-check-if-the-Phone-number-is-assigned-to-a-user?)  
   * [3\. How to check if 'Ring user assigned to called number' is checked or not?](#3.-How-to-check-if-'Ring-user-assigned-to-called-number'-is-checked-or-not?)  
   * [ ](#%C2%A0)  
   * [4\. How to check if the contact/lead inbound call number is assigned to a user?](#4.-How-to-check-if-the-contact/lead-inbound-call-number-is-assigned-to-a-user?)  
   * [5\. How to check if 'Forward calls to business phone number' is checked or not?](#5.-How-to-check-if-'Forward-calls-to-business-phone-number'-is-checked-or-not?)  
   * [6\. If you already checked, no Phone number is assigned to the users, no forwarding number configured, the call still forwards, why?](#6.-If-you-already-checked,-no-Phone-number-is-assigned-to-the-users,-no-forwarding-number-configured,-the-call-still-forwards,-why?)  
   * [7\. What happens if I don't configure any forwarding numbers?](#7.-What-happens-if-I-don't-configure-any-forwarding-numbers?)  
   * [8\. Can I configure the Phone number to go to a voicemail directly?](#8.-Can-I-configure-the-Phone-number-to-go-to-a-voicemail-directly?)  
   * [9\. I always want calls to forward to one number no matter what, how do I set this up?](#9.-I-always-want-calls-to-forward-to-one-number-no-matter-what,-how-do-I-set-this-up?)  
   * [10\. When we call the Phone number, it disconnects right away, and it won't even ring, we already reset and bought a new number but it's still showing the same issue?](#10.-When-we-call-the-Phone-number,-it-disconnects-right-away,-and-it-won't-even-ring,-we-already-reset-and-bought-a-new-number-but-it's-still-showing-the-same-issue?)  
   * [11\. Can we do call forwarding with an extension?](#11.-Can-we-do-call-forwarding-with-an-extension?)
  
  
Where do calls go when a lead calls back?
  
  
# Incoming Call to a Phone number

  
Incoming call to phone number forwarding depend on the user phone assignment / lead assignment or contact assigned to staff member. In this case staff profile call setting have vital role.  
  
**Below is the table to check the call flow for incoming call when user or lead is assigned to phone number or not**  
  
  
| Web App | Mobile App | User Phone Number | Phone Page Forwarding Number | Business Profile Phone No | Call Flow (Action)                                                     |
| ------- | ---------- | ----------------- | ---------------------------- | ------------------------- | ---------------------------------------------------------------------- |
| Yes     | Yes        | Yes               | Yes                          | Yes                       | Call will be forwarded to web/mobile/user phone number                 |
| Yes     | Yes        | Yes               | Yes                          | No                        | Call will be forwarded to web/mobile/user phone number                 |
| Yes     | Yes        | Yes               | No                           | Yes                       | Call will be forwarded to web/mobile/user phone number                 |
| Yes     | Yes        | Yes               | No                           | No                        | Call will be forwarded to web/mobile/user phone number                 |
| Yes     | Yes        | No                | No                           | No                        | Call will be forwarded to web app/mobile app                           |
| Yes     | No         | No                | No                           | No                        | Call will be forwarded to web                                          |
| Yes     | Yes        | No                | Yes                          | Yes                       | Call will be forwarded to web/mobile/ and phone page forwarding number |
| Yes     | Yes        | No                | No                           | Yes                       | Call will be forwarded to web/mobile/ and business phone number        |
| No      | No         | Yes               | Yes                          | Yes                       | Call will forward to user phone number                                 |
| No      | No         | Yes               | No                           | No                        | Call will forward to user phone number                                 |
| No      | No         | Yes               | Yes                          | No                        | Call will forward to user phone number                                 |
| No      | No         | No                | No                           | No                        | Call will drop immediately as no forwarding is there                   |
| No      | No         | No                | Yes                          | Yes                       | Call will forward to phone page forwarding number                      |
| No      | No         | No                | No                           | Yes                       | Call will forward to business phone number                             |
| Yes     | No         | No                | No                           | No                        | Call will forward to web app                                           |
| No      | Yes        | No                | No                           | No                        | Call will forward to mobile app                                        |
  
  
# **FAQs:**

  
## **1\. How would we know which Phone number the contact call if we have more than one Phone number?**

  
Go to **Conversations** \> Look up the contact > Hover over the Inbound call to click on the three dots > Click on **Details**  

  
![](https://s3.amazonaws.com/cdn.freshdesk.com/data/helpdesk/attachments/production/155031126630/original/2AqmZjuM4uOEoewZ-MmJRWWv3dxr-qhFaQ.png?1723760431)

  
To: You can view which Phone number the contact called here:

**![](https://s3.amazonaws.com/cdn.freshdesk.com/data/helpdesk/attachments/production/155031126652/original/pQdzPFPqVeIBljToR7G-2a1H8wKp0KwHNw.png?1723760535)**  

---
  
  
## **2\. How to check if the Phone number is assigned to a user?**

  
 Once you are in the sub-account, Click **Settings** at the bottom left**:**

![](https://s3.amazonaws.com/cdn.freshdesk.com/data/helpdesk/attachments/production/155031127421/original/6kMzndKB4jw5GLakQVMdkoxXJCFAqgbeLg.png?1723764448)

Click on **My Staff >** Click on **Edit** (pick any one user to edit)

![](https://s3.amazonaws.com/cdn.freshdesk.com/data/helpdesk/attachments/production/155031127415/original/rc-ET-1SdKZE2c2ygOYPn8-xRs0Nkmh6Cg.png?1723764416)
  
  
Expand **Call & Voicemail Settings**

Once you click the **Select Phone Number** dropdown

* If it says **Phone number (already assigned to another user)** and you don't know which user it is, the only way to check will be to Edit each user to Expand _Call & Voicemail Settings_ section to find out which user the number is assigned to.

![](https://s3.amazonaws.com/cdn.freshdesk.com/data/helpdesk/attachments/production/155029906795/original/kjhWIybQJmsrIhn0jRAGmpiC6ljHxJw1Rg.jpg?1721933465)

  
If you see a Phone number like this, e.g. my Phone number is (778) 907-0712

![](https://s3.amazonaws.com/cdn.freshdesk.com/data/helpdesk/attachments/production/155029906813/original/Emia26C6jgW0DZhauMVcayyBIwJZ3i5WRA.jpg?1721933510)

That means all calls to the assigned Phone number (778) 907-0712 will be routed to this **user's phone number**.

  
Even if the lead is assigned to another user, inbound calls will always always always go to the user's phone number.

  
Check what the user phone number is > Expand **User Info** in the first section to check the **user phone number**.

If there's no user phone number, it will fall back to the forwarding number set in phone number settings.

![](https://s3.amazonaws.com/cdn.freshdesk.com/data/helpdesk/attachments/production/155029906835/original/i5OTyVajw910opiu26C-hS0Ada8V2k8YIg.jpg?1721933554)

##   

## **3\. How to check if 'Ring user assigned to called number' is checked or not?**

You can see this option under Sub-account view > Settings > Phone Numbers > Advanced Settings > Voice Calls > Inbound Call ![](https://s3.amazonaws.com/cdn.freshdesk.com/data/helpdesk/attachments/production/155029906879/original/pXXiBsnlnfyFFuYNiVrJgOECZf12HjY1Hg.jpg?1721933602)  

## 

## **4\. How to check if the contact/lead inbound call number is assigned to a user?**

Once you are in the sub-account, Click on **Contacts**

  
![](https://s3.amazonaws.com/cdn.freshdesk.com/data/helpdesk/attachments/production/155029906906/original/9zfmVvXPFIihQ2Kr-L1y2ANjn-waPps1QA.jpg?1721933666)

  
Lookup the phone number of the contact who called the Phone number on the top right Quick Search box![](https://s3.amazonaws.com/cdn.freshdesk.com/data/helpdesk/attachments/production/155029906918/original/YPS4nP-tEjvdsGdrEMhmsEKlgml3cd1-Bg.jpg?1721933707)

  
Click on the contact

![](https://s3.amazonaws.com/cdn.freshdesk.com/data/helpdesk/attachments/production/155029906931/original/Jnve5YjQhEfQpP_20qBsjcaOfS6uwnoXaw.jpg?1721933745)

  
Check if the contact is Assigned to any users on top

![](https://s3.amazonaws.com/cdn.freshdesk.com/data/helpdesk/attachments/production/155029906949/original/GRx5qXENBweJgJ22cqgbUl2rXgT0xxyt_Q.jpg?1721933785)  

If it's assigned to User A, all inbound calls will go to User A

  
But if the Phone number that the contact dialled is assigned to user B already - 1st priority where the Phone number is assigned to the user ([How to check](https://help.gohighlevel.com/support/solutions/articles/48000981432-inbound-call-routing-explained#2.-How-to-check-if-the-Twilio-number-is-assigned-to-a-user?)), all inbound calls will go to User B even if the contact is assigned to User A.
  
  
## **5\. How to check if 'Forward calls to business phone number' is checked or not?**

You can see this option under Sub-account view > Settings > Phone Numbers > Advanced Settings > Voice Calls > Inbound Call ![](https://s3.amazonaws.com/cdn.freshdesk.com/data/helpdesk/attachments/production/155029906989/original/b_JFDrfWYl85V7RYFW8aNjrB5yxfOr6J1A.jpg?1721933851)

  
## **6\. If you already checked, no Phone number is assigned to the users, no forwarding number configured, the call still forwards, why?**

  
Please check if there's a company Phone set in 

**Business Information > Company Phone**

  
![](https://s3.amazonaws.com/cdn.freshdesk.com/data/helpdesk/attachments/production/155029907025/original/0NXXOIC8KZKXvveSo80Wy07e3vqBFAQsoQ.jpg?1721933901)  

  
## **7\. What happens if I don't configure any forwarding numbers?**

The call will drop immediately after we call the Phone number. Also number is assigned to any staff member and web/mobile app forward is enabled call will forward to web and mobile app

  
## **8\. Can I configure the Phone number to go to a voicemail directly?**

You can configure the [Voicemail For Company And For Users](https://help.gohighlevel.com/en/support/solutions/articles/48001146671). 

  
One way might be to get a Google voice number with the voicemail configured and put it in the forwarding number.

  
Set the incoming call timeout to 1 second so it will drop the call faster in 2-3 rings.

  
Or you can assign the Phone number to a user and receive [Inbound Calling on Mobile APP](https://help.gohighlevel.com/en/support/solutions/articles/48001224659).

![](https://s3.amazonaws.com/cdn.freshdesk.com/data/helpdesk/attachments/production/155029907065/original/otHk9jsvCxqULOruojQNlj4BoqQ2_WvWTA.jpg?1721933980)

## **9\. I always want calls to forward to one number no matter what, how do I set this up?**

You can set up a new user, and assign the Phone number to the user. All the calls will always go to that user's phone number.

  
## **10\. When we call the Phone number, it disconnects right away, and it won't even ring, we already reset and bought a new number but it's still showing the same issue?**

Edit the Phone number and check if there are any custom values set up in the whisper message. Broken custom values will affect incoming calls and cause it to drop.

  
Another possible reason is that the Phone number might not be voice capable. In this article [How to check logs for a specific Call in Twilio](https://help.gohighlevel.com/en/support/solutions/articles/48001229978), it will navigate how to also check the Phone number's capabilities. ![](https://s3.amazonaws.com/cdn.freshdesk.com/data/helpdesk/attachments/production/155029907101/original/ichGvGlWDIfV-T6iVpK_qhAYXlxvvv3trQ.jpg?1721934040)

## **11\. Can we do call forwarding with an extension?**

Only when a Phone number is assigned to users. There’s an extension field next to user's phone number. All the calls will always go to that user's phone number.

![](https://s3.amazonaws.com/cdn.freshdesk.com/data/helpdesk/attachments/production/155029907118/original/IHUO00y-GNbrPLcPsoOVRhFve1PxlMlxXQ.jpg?1721934083)  
  
  
**Scenario:** A lead receives a SMS or call from a HighLevel campaign. The lead calls back the number they see on their caller ID, which is the phone number originally setup (seen in Settings -> Phone Numbers). _Where does the call go?_

  
**Company Phone (First Layer):**

  
_If there is no Call Forwarding Number and the lead is not assigned to a specific user via a user assigned campaign..._

the call will be forwarded to the Company Phone.

  
To update the Company Phone follow the steps below:

1. Click Settings on the client view.
2. Click Company.
3. Update the number found in the Company Phone field.
4. Click Update Company.

  
**Call Forwarding Number (Second Layer):**

  
_If there is a Call Forwarding Number and the lead is not assigned to a specific user via a user assigned campaign..._

the call will be forwarded to the Call Forwarding Number.

  
To update the Call Forwarding Number follow the steps below:

1. Click Settings on the client view.
2. Click Phone Numbers.
3. Update the Call Forwarding Number of the selected default outbound number.
4. Click Save.

  
**User Phone (Third Layer)**

  
_If the lead is assigned to a user via a user assigned campaign..._

the call will be forwarded to the User Phone.

  
To update the User Phone follow the steps below:

1. Click Settings on the client view.
2. Click Team Management.
3. Click Edit for the user who was assigned the lead.
4. Update the Phone field.
5. Click Save.
  
  