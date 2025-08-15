**Date Updated:** 2025-07-23T01:51:23.000Z

**TABLE OF CONTENTS**

* [Step 1: Login to your Twilio account and click on the URL to view phone numbers:](#Step-1%3A-Login-to-your-Twilio-account-and-click-on-the-URL-to-view-phone-numbers%3A)
* [Step 2: Click on a phone number to edit the configuration](#Step-2%3A-Click-on-a-phone-number-to-edit-the-configuration)
* [Step 3: Set the Routing region to ‘US1’ if not done already. ](#Step-3%3A-Set-the-Routing-region-to-%E2%80%98US1%E2%80%99-if-not-done-already.%C2%A0)
* [Step 4: Under 'Voice Configuration' set it to:](#Step-4%3A-Under-'Voice-Configuration'-set-it-to%3A)
* [Step 5: Under 'Messaging Service' set it to Routing region to ‘US1’ if not done already. ](#Step-5%3A-Under-'Messaging-Service'-set-it-to-Routing-region-to-%E2%80%98US1%E2%80%99-if-not-done-already.-%C2%A0)
* [Step 6: Messaging service: No input/change needed ](#Step-6%3A-Messaging-service%3A-No-input/change-needed%C2%A0)
* [Frequently Asked Questions](#Frequently-Asked-Questions)

  
If you use Twilio and not LC phone directly, you need to setup webhooks to be able to receive incoming calls, messages and call status updates. In this article, we will help you learn how to do that in your Twilio console.

  
**Why should we setup webhooks?**

For you to receive calls, messages or status updates on our platform, Twilio needs to communicate with our system: send the incoming call, message or status update to us. Webhooks allow us to do that.  
  
Please follow the below steps to setup webhooks on Twilio (for incoming calls, incoming messages and call status updates):

  
# **Step 1: Login to [your Twilio account](https://console.twilio.com/us1/develop/phone-numbers/manage/incoming) and click on the URL to view phone numbers:**

![](https://s3.amazonaws.com/cdn.freshdesk.com/data/helpdesk/attachments/production/155029960826/original/IZ7yENfP_hQPi6ZixShX8idVcNClaP-ADg.jpg?1722004804)  
  
  
# **Step 2: Click on a phone number to edit the configuration**

![](https://s3.amazonaws.com/cdn.freshdesk.com/data/helpdesk/attachments/production/155029960924/original/5hdNuHihO0Bn1Zs85z92bDr0JuQoEXYsOA.jpg?1722004841)  

  
# **Step 3: Set the Routing region to ‘US1’ if not done already.** ![](https://s3.amazonaws.com/cdn.freshdesk.com/data/helpdesk/attachments/production/155029961064/original/R_E313n-15o49amF5BgCVQHTQ_4k1_Lhyw.jpg?1722004928)

  
# **Step 4: Under 'Voice Configuration' set it to:**

![](https://s3.amazonaws.com/cdn.freshdesk.com/data/helpdesk/attachments/production/155029961145/original/5YoMJcESIuUpyhmxjqxQBVtQ9VPkgtQ6EA.jpg?1722004991)

* Configure with: Webhook, TwiML Bin, Function, Studio Flow, Proxy Service
* A call comes in: Webhook
* Use the following URL[](https://staging.services.leadconnectorhq.com/phone-system/voice-call/inbound)  
[https://services.leadconnectorhq.com/phone-system/voice-call/inbound](https://staging.services.leadconnectorhq.com/phone-system/voice-call/inbound)
* HTTP: HTTP POST
* Primary handler fails: No changes needed
* Call status changes > URL:[](https://services.leadconnectorhq.com/appengine/twilio/incoming%5Fcall%5Fstatus)  
<https://services.leadconnectorhq.com/appengine/twilio/incoming%5Fcall%5Fstatus>
* HTTP: HTTP POST
* Caller Name Lookup: Your choice, we recommend keeping this 'Enabled' to use lookup
* Click on the save configuration button
  
  
# **Step 5: Under 'Messaging Service' set it to Routing region to ‘US1’ if not done already.** ![](https://s3.amazonaws.com/cdn.freshdesk.com/data/helpdesk/attachments/production/155029961258/original/9T8Q6PHmgecj9Grpd_PjC990gM-p2iaMlw.jpg?1722005052)

  
# **Step 6: Messaging service: No input/change needed** 

  
![](https://s3.amazonaws.com/cdn.freshdesk.com/data/helpdesk/attachments/production/155029961331/original/BouCDaftFsJpbqCW0FAO9fRcce4KS06oRw.jpg?1722005087)

* Configure with: Webhook, TwiML Bin, Function, Studio Flow, Proxy Service
* A message comes in: Webhook
* Use the following URL  
[](https://services.leadconnectorhq.com/conversations/providers/twilio/inbound%5Fmessage)<https://services.leadconnectorhq.com/appengine/twilio/incoming%5Fmessage>[](https://services.leadconnectorhq.com/appengine/twilio/incoming%5Fmessage)
* HTTP: HTTP POST
* Primary handler fails: No input/change needed
* Click on the save configuration button

---

# **Frequently Asked Questions**

Currently no frequently asked questions. Submit feedback on this article to help is add questions to this section!

#   