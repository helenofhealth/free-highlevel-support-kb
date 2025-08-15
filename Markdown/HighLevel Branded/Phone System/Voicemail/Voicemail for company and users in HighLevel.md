**Date Updated:** 2024-09-06T06:25:11.000Z

This article provides a guide to setting up and managing voicemail in HighLevel. Whether you need to configure voicemail for your company or for individual users, this resource covers all the essential steps. You’ll learn how to record and upload voicemail greetings, manage voicemail settings for both company and user accounts, and enable email notifications for incoming messages. Follow these instructions to ensure your voicemail system is set up effectively and tailored to your needs.

##   

**TABLE OF CONTENTS**

* [How to record your own voicemail](#How-to-record-your-own-voicemail)
* [Where To Upload Voicemail Files](#Where-To-Upload-Voicemail-Files)
* [Where To Control Timeout Settings](#Where-To-Control-Timeout-Settings)
* [Troubleshooting Company Voicemail not working](#Troubleshooting-Company-Voicemail-not-working)
* [Frequently Asked Questions](#Frequently-Asked-Questions)
* [Related Articles](#Related-Articles)

---
  
  
# **How to record your own voicemail**

  
Google Record mp3 online. Pick a website and record your voicemail online:

![](https://i.ibb.co/D8XPMJJ/chrome-capture-2023-1-22-1.gif)

##   

# **Where To Upload Voicemail Files**

  
Voicemail files (mp3 format) can be set in two different places:

  
1) Voicemail For **Users** \- Sub-Account > **Settings** \> **My Staff** tab > **Edit** User > Expand **Call & Voicemail Settings** \> **Upload mp3/wav file**

  
**[Learn more on how to Assign Twilio Numbers to Users](https://help.gohighlevel.com/en/support/solutions/articles/48001152124)**

  
[If the contact is assigned to the user](https://help.gohighlevel.com/support/solutions/articles/48000981432-inbound-call-routing-explained#3.-How-to-check-if-the-contact/lead-inbound-call-number-is-assigned-to-a-user?) OR if the Twilio number is assigned to the user, when they call the Twilio number and user didn't pick up, we will play the User voicemail here

![](https://i.ibb.co/n0gjtDd/2023-1-22-14-13-39.gif)
  
  
2) Voicemail For The **Business** \- Sub-Account > **Settings** \> **Business Profile** tab > Scroll down to **Call & Voicemail Settings** \> **Upload mp3/wav file**

  
When the contact calls the Twilio number that's not assigned to any users, and if the contact is also not assigned to any users, we will play the Voicemail For The **Business** if no one picks up.

![](https://i.ibb.co/g41HLtJ/2023-1-22-14-5-41.gif)
  
  
## How does it work?

  
When contact calls the Twilio number, we will ring the forwarding number for 10 seconds based on the call timeout set, after 10 seconds, if no one picks up, the contact will hear the voicemail recording.

  
Make sure Call Recording is enabled:

![](https://s3.amazonaws.com/cdn.freshdesk.com/data/helpdesk/attachments/production/155032366580/original/5aEHZ3pKu46WD9eU8dBn6qcIZpbWqqtAvw.jpg?1725583965)
  
  
Click on **Reporting** \> **Call Reporting** \> Scroll to the right and click on the arrow down button to expand each call
  
  
![](https://i.ibb.co/bghDVhz/2023-1-22-14-33-31.gif)
  
  
You can also click on the contact name to listen to the recordings in the **C** **onversation** page.

  
![](https://s3.amazonaws.com/cdn.freshdesk.com/data/helpdesk/attachments/production/155032366602/original/2FJlKMJKck1P2D5GV8UGesmeLadTXy1U5g.jpg?1725584034)
  
  
# **Where To Control Timeout Settings**

  
To replace the original voicemail of the forwarding number, you'll need to set a "Timeout" number, otherwise, the call will ring by default for 60 seconds, during which time the original voicemail of the forwarding number will usually trigger and we will not be able to replace it with the uploaded recorded voicemail.

  
Timeout numbers can be set in three different places:

  
1) Sub Account > Settings > Team Management tab > Edit user > Call & Voicemail Settings

2) Sub Account > Settings > Phone Numbers > Pencil Icon for a specific phone number

3) Sub Account > Settings Company Tab
  
  
**Understanding Priorities For Timeout Settings:**

  
When a call comes into a Twilio number, it will ring for 60 seconds by default before looking for a voicemail to play unless a Timeout number has been set. HighLevel will look for timeout number in the following order:

  
First - is there a Timeout number in the user settings of the user this Twilio number is attached to? (option 1 above)

Second - is there a Timeout number in the phone number settings of this number? (option 2 above)

Third - is there Timeout number in the Company settings? (option 3 above)

  
**Other Notes:** 

  
If a call comes into a Twilio number and a Timeout number is found but no voicemail files are found, the following default message will be played: "**We are unable to take your call right now. Please leave a message after the beep**."

  
Timeout numbers are not "connected" with any particular voicemail file, e.g. a call comes into a Twilio number and HighLevel detects a timeout number set in the User's settings (but that user doesn’t have a voicemail file) and HighLevel finds a voicemail file in the Business Profile settings, HighLevel will play the voicemail file from the Business Profile settings after the number of seconds set in the Timeout field in the User's settings. 
  
  
# **Troubleshooting Company Voicemail not working**

  
### 1\. Check if the Twilio number is assigned to the user, and make sure the user has uploaded a voicemail file.

  
![](https://s3.amazonaws.com/cdn.freshdesk.com/data/helpdesk/attachments/production/155032366499/original/Zb1gZ7RCDgUZxWEZHwIJ9LSrrnTKpjejFA.png?1725583293)

  
### 2\. Check if there's any **forwarding number / Business phone** configured, we will need to forward the call somewhere in order to drop/play the uploaded voicemail.

  
\- One way might be to get a Google voice number and put it in the forwarding number. Set the incoming call timeout to 1 second so it will drop the call faster in 2-3 rings. The call timeout will need to be at least 1 second to attempt to connect the call. The idea is to drop/time out the call before the forwarding number's original voicemail is played. 

  
\- Or you can assign the Twilio number to a user and receive [Inbound Calling on Mobile APP](https://help.gohighlevel.com/en/support/solutions/articles/48001224659).
  
  
### 3\. Check the call timeout set, try setting the Inbound call timeout to 1 second

  
The maximum Incoming Call Timeout should be less than 20 seconds. If the call timeout is set to be more than 20 seconds, we won't be able to replace the original voicemail as usually the original voicemail of the forwarding number will be playing by the time.

  
If it's already set to 20 seconds but it's still playing the forwarding number's original voicemail instead of the voicemail you uploaded, try setting the call timeout to 1 second and try calling again to see if it works. If it works, you can gradually increase the call timeout (10 seconds, 15 seconds) to test further so it will call the forwarding number for a longer time and still be able to play the uploaded voicemail.
  
  
![](https://s3.amazonaws.com/cdn.freshdesk.com/data/helpdesk/attachments/production/155032366625/original/6xtEE7zhc9ns1cyOkb6yfqeQOhH8V4csag.jpg?1725584102)
  
  
### 4\. Check if we call the forwarding number directly, does the call go to a voicemail as soon as you call it?

  
If the forwarding number is in Do Not Disturb mode or if the number is configured to go directly to a pre-set voicemail. In that case, we won't be able to replace that voicemail because the forwarding number's original voicemail just plays immediately.

  
The key is to figure out how soon your own voicemail will play and set the call timeout to drop the call before your voicemail answers. If your voicemail answers right away during Do Not Disturb mode, then we won't be able to replace the original voicemail.

###   

If you are using a Google voice number or landline, they might have their own call settings so we are not able to overwrite their configured voicemail. You may have to turn off the announce feature in Google Voice. That may pick up as a voicemail and we are not able to overwrite its original voicemail.

###   

  
### 5\. Check if the uploaded Voicemail file is too high quality

  
If the voicemail file quality is high and also not an mp3 file, these instructions should help you make it compatible

1\. go to <https://online-audio-converter.com/> and upload the voicemail file 

2\. Convert to ECONOMY 64kbps MP3 

3\. Upload it and call the Twilio number to test again 

  
---

# **Frequently Asked Questions**

Currently no frequently asked questions. Submit feedback on this article to help is add questions to this section!

---

# **Related Articles**

* [](https://help.gohighlevel.com/en/support/solutions/articles/155000002369)[How to use voicemail in workflows](https://help.gohighlevel.com/support/solutions/articles/155000003275-workflow-action-voicemail)
* [How to setup and use voicemail drops ](https://help.gohighlevel.com/support/solutions/articles/48000981430-call-voicemail-drop-events)

  