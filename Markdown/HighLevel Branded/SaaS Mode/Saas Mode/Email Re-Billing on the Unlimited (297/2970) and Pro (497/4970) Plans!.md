**Date Updated:** 2024-09-17T02:59:05.000Z

Email Rebilling is a valuable feature for SaaS platforms, enabling agencies to automatically markup and charge clients for email-related costs. This creates an additional revenue stream for agencies while providing better control over client email usage. The client's payment card details are required to facilitate smooth rebilling and prevent unauthorized configuration changes.

  
**TABLE OF CONTENTS**

   * [What is Email Rebilling?](#What-is-Email-Rebilling?)
   * [Good Use Cases for this feature](#Good-Use-Cases-for-this-feature%3A)
   * [To Enable Email Re-Billing](#To-Enable-Email-Re-Billing)[](#Frequently-Asked-Questions)[](#Related-Articles)
   * [Related Articles](#Related-Articles)

#### [](#FAQs)

  
---

## **What is Email Rebilling?**

  
**Please Note:**

Email Rebilling is available for agencies on the $497/$4970 plans and Agencies on the $297/$2970 Unlimited Plan can also rebill email costs to sub-accounts.
But for the $297/$2970 plans it Only works with the LeadConnector SMTP with a fixed markup of 1.05x. Sub-account should have a payment method added for this rebilling to work. They will not be allowed to change their SMTP once rebilling has been enabled.

  
Email Rebilling is a feature offered by the CRM that allows agencies to automatically markup and charge their clients for email-related costs incurred while using the platform. This feature enables agencies to generate incremental revenue by reselling email services to their clients.

  
When an agency enables email rebilling in their SaaS configurator, the system can automatically apply it to new and existing SaaS accounts. The agency can set a multiplier to determine the markup on email costs, which is then passed on to their clients.

  
To enable email rebilling for a client, the client must have their payment card details added to the platform. The agency can then charge the client for the email services, covering the base email cost and generating a profit.

  
Email rebilling provides agencies with better control over client email usage and costs, while also preventing double billing or unauthorized changes to the email service configuration. Additionally, agencies can be notified via email and SMS when a rebilling charge fails, ensuring better visibility and management of their client's rebilling payments.

  
## **Good Use Cases for this feature**

**Digital Marketing Agencies:** Agencies that manage email marketing campaigns for multiple clients can use email rebilling to charge clients for the emails sent on their behalf, including the base cost and a profit margin.

  
**Software Development Companies:** Companies that provide custom-built SaaS solutions can enable email rebilling to charge clients for transactional and notification emails sent through the platform, ensuring a steady revenue stream.

  
**E-commerce Businesses:** E-commerce platforms that offer white-label solutions to online retailers can use email rebilling to charge clients for promotional and transactional emails sent to their customers.

  
**CRM Providers:** CRM (Customer Relationship Management) platforms that handle email communications for sales and support teams can leverage email rebilling to charge clients based on their email usage, while also managing the email service configurations on their behalf.

  
**Event Management Platforms:** Platforms that manage event registrations and communications can use email rebilling to charge event organizers for the emails sent to attendees, such as invitations, confirmations, and reminders.

  
**Online Course Providers:** Educational platforms that offer online courses can enable email rebilling to charge clients (instructors or institutions) for emails sent to students, including course updates, announcements, and notifications.

  
**Membership Platforms:** Platforms that manage memberships for clubs, associations, or organizations can use email rebilling to charge clients for member communications, such as newsletters, event invitations, and renewal reminders.

  
---

## **To Enable Email Re-Billing**

1\. If the sub-account isn't in SaaS Mode already

Once you are in the agency view, click on **Sub-Accounts** \> Search by **sub-account**

  
![](https://s3.amazonaws.com/cdn.freshdesk.com/data/helpdesk/attachments/production/155032967225/original/0VwqmhavyPY9KJGkGXJz5ZcotgUeb02ILw.jpg?1726521885)

  
2\. Click the three dots icon and select "Switch to SaaS"

  
![](https://s3.amazonaws.com/cdn.freshdesk.com/data/helpdesk/attachments/production/155032967227/original/t-DkNZhlrk5IgpWM_Safl87iztp_RcygsA.jpg?1726521920)

  
3\. Click on the **sub-account Name** _OR_ click on the three dots at the bottom right to **Manage Client**

  
![](https://s3.amazonaws.com/cdn.freshdesk.com/data/helpdesk/attachments/production/155032967231/original/gIMXfnVO9cgP-tD5UgWhTIe5SPvgcv-wPw.jpg?1726521979)

  
4\. Input your original email cost (If you're on the $35/month Mailgun plan, your cost should be approximately $0.007 per email)

  
Scroll down to find the **Email Resell Settings** section.

  
5\. Use the slider to set the amount of markup you like to make and hit save!

  
![](https://s3.amazonaws.com/cdn.freshdesk.com/data/helpdesk/attachments/production/155032967252/original/Qi08OuMmlpyMoV-b87Gf0ScwPPi9iyZflw.jpg?1726522060)
  
  
---

# **Frequently Asked Questions**
  
  
### **Why the Add Service button is missing?**

  
Disabling the feature will allow us to make edits to the SMTP settings. [Please disable email rebilling following the steps here](https://help.gohighlevel.com/en/support/solutions/articles/48001207525).

Because clients should not be using their own SMTP when email rebilling is enabled, as that should work with Mailgun only, switching it on and off won't automatically delete what is set up there. But the idea is that we don't allow edits to update the SMTP integration easily here.

  
### **How do I determine my email cost to enter the "Your email cost" field?**

  
Log into your SMTP provider, navigate to the Plan or Billing section, and look for a description of how many emails are included in your plan. Once know the number of emails in your plan, divide that by the cost of your plan, and the result will be your email cost. For example, the $35/month Mailgun plan includes 50,000 emails, so 35/50000= email cost of $0.0007
  
  
### **How do I change the default Mailgun domain used for my SaaS Mode clients?**

  
By default, the email from your SaaS Mode sub-accounts will be sent from the default sending sub-domain as configured in your Agency account settings > Mailgun tab. You can override the default per-subaccount by going into the sub-account settings > SMTP tab and adding a different SMTP provider. 
  
  
### **Can a SaaS client who spams from their sub-account burn my domain? Should I get a generic domain instead?**

  
Using a generic domain is recommended so you don't risk your clients damaging the reputation of your agency's main domain.
  
  
### **What if I wish to use my client's brand domain at a later stage?**

  
You can configure a sub-account to send emails from any SMTP provider by visiting the sub-accounts settings > SMTP tab. 
  
  
### **Does email rebilling pull from a different wallet than Twilio rebilling?**

  
No, both email & Twilio rebilling work from the same wallet.
  
  
### **Will there be two invoices now -** **one for email and one for Twilio?**

  
No, invoices combine both email and Twilio usage. 
  
  
---

# **Related Articles**

* [Rebilling, Reselling, and Wallets Explained](https://help.gohighlevel.com/support/solutions/articles/155000002095-rebilling-reselling-and-wallets-explained)
  
  