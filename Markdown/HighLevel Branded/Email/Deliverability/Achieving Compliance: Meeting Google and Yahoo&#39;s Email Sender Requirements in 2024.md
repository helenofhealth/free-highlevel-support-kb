**Date Updated:** 2024-01-24T05:07:23.000Z

From February 2024 onwards, [Google](https://blog.google/products/gmail/gmail-security-authentication-spam-protection/) and [Yahoo](https://blog.postmaster.yahooinc.com/post/730172167494483968/more-secure-less-spam) are making it necessary for email senders to use email authentication, and there are also some important policy changes related to consent and engagement. If senders don't follow these rules, their emails might be delayed, blocked, or marked as spam. Even though this might feel like a sudden change, these requirements have actually been considered the best way to make sure emails get delivered properly for quite some time.

  
**TABLE OF CONTENTS**

  
[1\. Elevate Your Brand with a Branded Sending Domain](#1.-Elevate-Your-Brand-with-a-Branded-Sending-Domain)

[2\. Establish DMARC Email Authentication for Your Sending Domain](#2.-Establish-DMARC-Email-Authentication-for-Your-Sending-Domain)

[3\. Ensure Brand Consistency](#3.-Ensure-Brand-Consistency)

[4\. Avoid pretending to be Gmail in the "From" headers of your emails](#4.-Avoid-pretending-to-be-Gmail-in-the-)

[5\. Make it easy to Unsubscribe](#5.-Make-it-easy-to-Unsubscribe)

[6\. Optimize Email Delivery: Keep Your Spam Rate Below 0.30%](#6.-Optimize-Email-Delivery%3A-Keep-Your-Spam-Rate-Below-0.30%)

---

## **Prepare Your Account:**

Follow our checklist to make sure you meet the new sender requirements set by both Google and Yahoo.

  
### **1\. Elevate Your Brand with a Branded Sending Sub-Domain**

Enhance control over your sender reputation and improve inbox branding by setting up a branded sending sub-domain. Say goodbye to the "sent via msgsndr.com" disclaimer and embrace better deliverability practices. Starting in February, this becomes a must for bulk senders reaching out to Google and Yahoo recipients. 

  
Keep in mind that after enabling your branded sending sub-domain, a [gradual warm-up of your sending infrastructure](https://help.gohighlevel.com/en/support/solutions/articles/155000001021) may be necessary over the next 2 – 4 weeks. 

  
Need assistance? Check out our guide on [setting up a branded sending sub-domain](https://help.gohighlevel.com/en/support/solutions/articles/48001226115).

  
_Example of what a Branded sending domain looks like to Gmail users_

![](https://s3.amazonaws.com/cdn.freshdesk.com/data/helpdesk/attachments/production/155016475064/original/8uoY_YI_Ye80dKWg-qd3wzOmdMQ_2y8xrQ.png?1704091630)

  
---

### **2\. Establish DMARC Email Authentication for Your Sending Domain**

  
What is DMARC? DMARC, short for Domain-based Message Authentication, Reporting & Conformance, is a standard that enhances SPF and DKIM. It communicates a policy to mailbox providers, guiding them on how to handle emails failing SPF, DKIM, or both, claiming to be from your domain (potentially spoofed).

  
What should you do? **If you lack a DMARC record AND are** **sending more than 5,000 emails per day** (aggregated for sub-accounts using a shared sending domain), you should add one to your DNS. 

  
**Implementation Steps:**

1\. Use a free DMARC checker like [Dmarcian](https://dmarcian.com/dmarc-inspector/) to find out if you already have a DMARC record in place. Enter your root domain (ie: yourdomain.com) and hit inspect. If you see "Hooray! Your DMARC record is valid.", you're good to go - ignore the following steps. _If not, continue to step 2\._ 

2\. Visit your DNS hosting provider and create a TXT DNS record.

3\. Choose **TXT as the record type**.

4\. Set the Host/Name value as: **\_DMARC** 

5\. In the Content/Points to field, enter: **v=DMARC1; p=none;**

  
Keep in-mind that Google recommends gradually changing your DMARC policy over time to be more restrictive. You can read about this process in their [Recommended DMARC Rollout Tutorial](https://support.google.com/a/answer/10032473?hl=en) document.

  
Here's what the record would look like if setting up in Cloudflare for a domain called demohighlevel.com:

  
![](https://s3.amazonaws.com/cdn.freshdesk.com/data/helpdesk/attachments/production/155016936712/original/q2kS5_X1ohoU4kk0xYGq4P5jK9p8K-aKww.png?1704484436)

  
6\. Save/submit and use [Dmarcian](https://dmarcian.com/dmarc-inspector/) to verify the DMARC record has successfully been added (it may take a few minutes to register). You can also check by sending yourself an email and inspecting the header. 

  
In Gmail, you can inspect the header of an email by clicking the three-dots icon and selecting the "Show More" option. Here's what the header will look like for an email that was sent from a domain that has a valid DMARC record in place:

![](https://s3.amazonaws.com/cdn.freshdesk.com/data/helpdesk/attachments/production/155016475267/original/LsZGJkzJ7Xz7bQ8lNqMeRAK0HeLAWQ5J2Q.png?1704091825)

---

### **3\. Ensure Brand Consistency**

**Align your "from" address with your branded domain for a cohesive and recognizable email identity.**

  
To align with DMARC standards, your "from" address domain must match the root domain of your branded sending domain. For example, if your branded sending domain is "lc.msgsndr.com," the corresponding root domain is "msgsndr.com." Thus, using "hello@msgsndr.com" as your "from" address maintains alignment with the root domain.

  
Double-check all "from" addresses in your flow emails and campaigns to ensure alignment. 

  
**Remember, if you're a bulk sender, you must transition to a branded sending domain by February 2024.**

---

### **4\. Avoid pretending to be Gmail in the "From" headers of your emails**

  
**Why does it matter?** 

Gmail and Yahoo is getting stricter with a DMARC policy called 'quarantine.' If you try to act like you're sending from Gmail or Yahoo, it could harm how your emails get delivered.

  
**What's the solution?** 

Keep it simple: just don't pretend to be Gmail or Yahoo in the "From" part of your emails. To put it briefly, don't send emails claiming to be from 'example@gmail.com' or 'example@yahoo.com'.

---

### **5\. Make it easy to Unsubscribe**

  
Now, it's important for senders to make it really easy for people to stop getting their emails. If someone doesn't want the emails anymore, they shouldn't have to search for the unsubscribe button.

  
If you use LC Email Service, [take a look at this blog post](https://help.gohighlevel.com/en/support/solutions/articles/48001225534). Turning on this option will automatically include an unsubscribe link in the footer of all your emails.

###   

**Streamlined Unsubscribing: One-Click Solution**

  
We've got good news for you! Meeting the new requirement of having a one-click unsubscribe link in every email just got easier with us. They've got it covered for you by automatically adding a one-click unsubscribe link to the header of each email you send except 1:1 emails.

  
Just to clarify, the "header" here refers to the behind-the-scenes information in your email, which includes details about the sender and message authentication. We are enhancing the one-click list-unsubscribe feature in the code for every message. While the appearance of one-click unsubscribe may vary in different email platforms, a visual example from Gmail is shown below.

  
_Example of what one-click unsubscribe looks like to Gmail users_

![](https://s3.amazonaws.com/cdn.freshdesk.com/data/helpdesk/attachments/production/155016474638/original/4ZRftmRvW6v6Gh8vyGsD0TvQrLh7a_UcVA.png?1704090848)

  
Your only task? Before February rolls around, take a quick look at all your campaign templates and flow emails. Ensure there's an unsubscribe link somewhere in your email body – the footer is typically a common spot. It doesn't have to be one-click, but it should be clear and easy for recipients to find. Easy as that!

---

### **6\. Optimize Email Delivery: Keep Your Spam Rate Below 0.30%**

Make Sure People Want Your Emails: Just like you wouldn't want a stranger in your home without permission, it's not cool to send emails without permission either. Always make sure that people actually want to get emails from you.

  
If too many people complain about your emails being spam (like 3 out of every 1,000), it can cause problems. Your emails might get delayed, end up in the spam folder, or not get delivered at all. To avoid this, try to keep your spam complaints to less than 1 out of every 1,000 emails you send.

  
You can check Yahoo spam complaints in the Spam Reports. But, remember, we cannot track Gmail spam complaints and as such they are not included in email metrics within HighLevel. Gmail has its way of handling spam complaints to keep user info private. If you want to keep an eye on Gmail spam complaints, use [Google Postmaster Tools](https://www.gmail.com/postmaster/). This helps make sure your emails get to where they're supposed to go without any issues.