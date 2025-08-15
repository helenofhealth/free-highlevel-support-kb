**Date Updated:** 2023-09-16T00:41:56.000Z

The Facebook Lead Ads integration allows you to collect leads directly from Facebook Ads and have them automatically synced with your CRM. With this integration, you can easily capture contact information from potential customers interested in your products or services on Facebook and quickly follow up with them through your CRM. By automating the lead capture process, you can save time and improve the efficiency of your sales and marketing efforts.

  
#### **Covered in this Article:**

#### [**What is the Facebook Lead Ads Integration?**](#What-is-the-Facebook-Lead-Ads-Integration?)

#### [Who is this integration helpful for?](#Who-is-this-integration-helpful-for?)

#### [What are the benefits of this integration?](#What-are-the-benefits-of-this-integration?)

####   
[**Pre-requisites for Facebook Lead Ads**](#Pre-requisites-for-Facebook-Lead-Ads)

#### [Supported custom fields when using Facebook Lead Ads:](#Supported-custom-fields-when-using-Facebook-Lead-Ads%3A)

####   
[How to directly integrate Facebook Leads Ads with a Sub-Account](#How-to-directly-integrate-Facebook-Leads-Ads-with-a-Sub-Account)

####   
[**Troubleshooting**](#Troubleshooting)

#### [Why are my Lead Ads not making it into my Sub-Account?](#Why-are-my-Lead-Ads-not-making-it-into-my-Sub-Account?)

#### [How do I integrate Facebook Leads using a 3rd party service like Pabbly Connect or Zapier?](#How-do-I-integrate-Facebook-Leads-using-a-3rd-party-service-like-Pabbly-Connect-or-Zapier?)

#### [A Facebook Token Has Expired In a Sub-Account; why does this happen, and How to Fix This?](#A-Facebook-Token-Has-Expired-In-a-Sub-Account;-why-does-this-happen,-and-How-to-Fix-This?)

####   
[**Common Errors**](#Common-Errors)

#### [Page Quality Issue](#Page-Quality-Issue-%3A%C2%A0)

#### [Permission Issue](#Permission-Issue%3A%C2%A0)

#### [Instagram Connection/messages Check](#Instagram-Connection/messages-Check%3A)

#### [Messenger/ Instagram not syncing all messages](#Messenger/-Instagram-not-syncing-all-messages%3A)

#### [Leads, not syncing Issue](#Leads,-not-syncing-Issue%3A)

#### [How to connect Instagram Account to the FB page or verify it is connected](#How-to-connect-Instagram-Account-to-the-FB-page-or-verify-it-is-connected%3A)

#### [Missing Pages](#Pages-Missing)

#### [](#Zapier-Flow%3A%C2%A0)

---

## **What is the Facebook Lead Ads Integration?**

The Facebook Lead Ads integration with a CRM (Customer Relationship Management) system allows businesses to capture and automatically import leads generated through Facebook Ads into their CRM system. This integration enables businesses to streamline their lead capture process, avoid manual data entry errors, and follow up with leads more efficiently. By integrating Facebook Lead Ads with a CRM, businesses can track and manage their leads through a single platform, which can improve Lead quality, increase conversions, and ultimately help grow their business**.** 
  
  
### **Who is this integration helpful for?**

The Facebook Lead Ads integration with a CRM can be beneficial for any business or organization that is using Facebook Ads to generate leads and wants to streamline their lead capture process. It can benefit small businesses or startups that may not have a large sales or marketing team to collect and manage leads manually. By automating the lead capture process, businesses can save time and resources while improving their lead data's accuracy and quality. Additionally, the integration can benefit businesses already using a CRM by seamlessly integrating their Facebook lead data into their existing workflows and follow-up processes.

  
### **What are the benefits of this integration?**

The benefits of integrating Facebook Lead Ads with the CRM include:

  
**Automated lead capture:** With this integration, businesses can automatically capture leads generated through Facebook Ads and import them into their CRM system, eliminating the need for manual data entry. 

  
**Improved Lead Quality:** By tracking and managing leads through CRM, businesses can better understand their audience, personalize their marketing efforts, and improve the overall quality of their leads. 

  
**Enhanced lead management:** The CRM system allows businesses to track and manage their leads in one place, providing a 360-degree view of their interactions with prospects and customers. This can help companies to streamline their sales and marketing efforts and improve customer retention.

  
**Efficient follow-up:** With lead data automatically captured and imported into the CRM system, businesses can quickly follow up with leads and prioritize their sales efforts based on lead quality and behavior.

  
**Increased conversions:** Businesses can increase their conversions and ROI from Facebook Ads by automating lead capture and improving lead management.

  
---

## **Pre-requisites for Facebook Lead Ads**

* **Access**: You must have access to the Facebook page for which you're creating lead ads. Refer to this Facebook Help article on [how to give someone a role on your Page](https://www.facebook.com/help/187316341316631).
* **Ownership:** Ensure the same user owns the page and the ad account. For business-level integrations, the owner of the page and the ad account must be the same—more on this in the Facebook help section on [Ad account roles](https://www.facebook.com/business/help/187316341316631?id=520795622598421).
* **Permissions:** Verify that you have the page and ad account permissions. You should ideally have admin or manage permissions. To understand different levels of permissions, refer to [Facebook Pages roles](https://www.facebook.com/help/323502271070625) and [Ads permissions](https://www.facebook.com/business/help/187316341316631?id=520795622598421). The user trying to integrate the Facebook Page into the CRM will **[need to be an admin of the Facebook Business page](https://www.facebook.com/business/help/2169003770027706?id=2190812977867143)** and have [**Lead Access Permission**](https://www.facebook.com/business/help/540596413257598?id=735435806665862) to access Lead data (A requirement set by Facebook).
* **Ad Account Check:** Confirm your page is connected to the appropriate ad account. To do this, navigate to the Ad Account settings and verify the connected page—more on [how to navigate your ad account settings](https://www.facebook.com/business/help/337584869654348).
* **Visibility:** Note that only individuals with relevant permissions can see the owners of ad accounts. For details, check Facebook's guide on [user permissions for ad accounts](https://www.facebook.com/business/help/187316341316631?id=520795622598421).
* **Leads Access:** Check if you have lead access. If the lead connector isn't showing, you may need to manually search for it or enable it. For issues related to leads not syncing, refer to Facebook's [troubleshooting guide for lead ads](https://www.facebook.com/business/help/1667649039945425).
* LeadConnector will need access to the Facebook Business Manager and Business Page from which you run the Facebook Lead Ad.
* If you have moved your page to the [New Pages Experience](https://www.facebook.com/business/help/2752670058165459), You can allow trusted people to manage some of your Facebook business pages. You can give some people [access](https://www.facebook.com/business/help/582754542592549?id=418112142508425) to certain parts of your Facebook page without giving them full access.
* Open business manager > Left navigation > Users > People. If you have added the person, who will be integrating the FB page to the CRM, there already: they will appear at the center of the page.  
Click on the name and see more details, like the role. The role needs to have **Admin or Employee** access.  
    
If you have not added them, Please follow the steps to add people/users first.  
    
[How to add users to your business? ](https://www.facebook.com/business/help/2169003770027706?id=2190812977867143)  
    
Remember that this business manager role differs from Page Role; the Page Role must still be the **Admin.**  
    
**Please Note:**  
The new Pages experience isn't available for all Pages yet. Some Pages you manage might still use the classic Pages experience. [Learn more about classic Pages.](https://www.facebook.com/help/135275340210354)
* When creating the custom fields for the Lead Ad in the CRM, please make sure to use the supported custom fields listed below:

  
### **Supported custom fields when using Facebook Lead Ads:**

* TEXT
* LARGE\_TEXT
* NUMERICAL
* PHONE
* MONETARY
* SINGLE\_OPTIONS
* DATE
* DROPDOWN
* RADIO OPTIONS
* CHECKBOX

  
### ![](https://s3.amazonaws.com/cdn.freshdesk.com/data/helpdesk/attachments/production/48251510706/original/pEmtn9V_VcLgRYSW4mOGfvvGEH3FvTaupA.gif?1663348062)  
  
  
---

## **How to directly integrate Facebook Leads Ads with a Sub-Account**
  
  
**Please Note:**

Only the User that integrated the FB page will be able to see that page in the dropdown of pages. They need to be the admin of that FB page to see it in the dropdown of pages and will no longer see other accounts' FB Pages in the list.![](https://s3.amazonaws.com/cdn.freshdesk.com/data/helpdesk/attachments/production/48291400274/original/g41sAjRNyGtEtdYy-9Cv6ezS7sGvCqVccA.png?1680771876)

  
Facebook form mapping has moved under location **settings > integrations > Facebook Form Field Mapping.**

![](https://s3.amazonaws.com/cdn.freshdesk.com/data/helpdesk/attachments/production/48245875992/original/zjZlJ3p2-QaSQiO4zraR-Bojc7vctxJRrg.gif?1660747191)
  
  
---

## **Troubleshooting**

  
### **Why are my Lead Ads not making it into my Sub-Account?**

1. Are you an admin of the Facebook page - [](https://www.facebook.com/business/help/294498964994409?id=418112142508425)[How to add an admin to my Business Manager](https://www.facebook.com/business/help/2169003770027706?id=2190812977867143)
2. Can you confirm that the correct _FB Lead Ad form_ is selected in your Facebook ads manager and matches the one in your Sub-Account? - <https://web.facebook.com/business/tools/ads-manager>
3. Now in your Sub-Account, **check in settings**\> **integrations** \> **Facebook form fields mapping** if there is a blue tick mark next to the form you have selected in ads manager.
4. If you are, in fact, the FB Admin, can you try this to confirm if Lead Connector is accessible and can allow access to your page?

  
**Link mentioned in the video** \- <https://www.facebook.com/settings?tab=business%5Ftools&ref=settings>
  
  
6\. Once you have completed the steps in the video above, please use the [**Facebook leads ads testing tool**](https://developers.facebook.com/tools/lead-ads-testing) to see if leads are now being added to your Sub-Account.

  
**Lead Ad Testing Tool:** <https://developers.facebook.com/tools/lead-ads-testing>  
**Facebook Page Select:** <https://app.gohighlevel.com/location/YOUR%5FLOCATION%5FID/facebook%5Fpage%5Fselect>
  
  
**Please Note:**

When testing are you able to locate the **App ID** **39018126477806?** (Mentioned in the video above @2:49 seconds)   
  
If the app ID does **not** show up, then LeadConnector does not have access. If that is the case please continue to **step 7 below**.  
  
If Facebook Lead Ads are not coming into the CRM Please try using unique contact info as explained in the video below:   
  
  
7\. If you see that LeadConnector access to your page has been revoked or the App ID is not coming up, you will manually need to assign Lead access permissions to LeadConnector on Facebook:

i. Go to Business Suite.

ii. If you don't have access to Business Suite, go to Business Settings and select your business, skip to step (v)

iii. Click the dropdown in the top-left corner and choose your business account.

iv. Click Settings in the bottom-left corner.

v. Click More Business Settings.

vi. Click Integrations in the left menu, then click Leads Access.

vii. Click Assign CRMs. You'll see a list of CRM systems integrated with your Facebook Page.

viii. Check the circle next to LeadConnector, then click Assign.

  
**Please Note:**

The Page Admin who granted permissions to LeadConnector must continue to have access permission or else LeadConnector will fail to fetch data.
  
  
### **How do I integrate Facebook Leads using a 3rd party service like Pabbly Connect or Zapier?**

You can use a 3rd parties integration tool like Zapier or Pabbly Connect. Here is [more info](https://help.gohighlevel.com/en/support/solutions/articles/48001223700)

  
### **A Facebook Token Has Expired In a Sub-Account; why does this happen, and How to Fix This?**

If you received an email with a subject that says "Important: Facebook connection has expired.", this means that the Facebook integration for one of your Sub-accounts has become disconnected.

  
**Why Did This Connection Break?**

  
Several reasons could cause the integration to break. The most common are: 

  
A user changes their password

The Facebook token naturally expires after some time

A user de-authorizes your app

A user logs out of Facebook

A user changes page permission or adds/removes a user

A virtual assistant in another country logs in without using a VPN

  
**To reconnect:**

  
1\. Select the account indicated in the email you received from the "Switch To An Account" dropdown

  
2\. In the left-hand sidebar, click "Settings."

  
3\. From the sidebar, click "Integrations."

  
4\. Click the "Connected" button to disconnect the broken integration under the Facebook icon. Click on Connect again to reconnect

  
5\. In the window that pops up, continue as yourself, select the Facebook page that you want to connect, then click the "Connect Page" button

---

## **Common Errors**

### **Page Quality Issue :** 

Suppose our user is facing this issue. Our customer needs to raise a support ticket with Facebook Support.

**Steps to resolve:**

* Users need to switch to the Facebook page on Facebook, Go to [this link](https://www.facebook.com/settings?tab=profile%5Fquality) and raise a support ticket with Facebook if there is an issue.
* [FB Support Doc:](https://www.facebook.com/help/1985220725104252)![](https://s3.amazonaws.com/cdn.freshdesk.com/data/helpdesk/attachments/production/155003144440/original/KaKuKPEP1cyXwgjBNcXM61Rt7C88UF_bkA.png?1689683139)

### **Permission Issue:** 

The easiest way to find the issues is by trying to fetch the latest FB/Insta message and the latest lead.

This is how Zapier does it, and it helps us easily find the missed permission. FB API will present an error if permission is missing or for other reasons. Troubleshooting steps are as follows:

* Go to [this link](https://www.facebook.com/settings?tab=business%5Ftools&ref=settings). [](https://www.facebook.com/settings?tab=applications&ref=settings)
* [And then this link](https://www.facebook.com/settings?tab=applications&ref=settings)
* Check if all the permission are enabled for all pages.  
![](https://s3.amazonaws.com/cdn.freshdesk.com/data/helpdesk/attachments/production/155003145086/original/BiczOlvBDQYiINfEVG-o8Kqmv50xUF_upQ.png?1689683477)

### **Instagram Connection/messages Check:**

Check Instagram page is connected to the FB page

* Switch your logged-in user to the desired Fb page and go to [this link](https://www.facebook.com/settings?tab=linked%5Finstagram).![](https://s3.amazonaws.com/cdn.freshdesk.com/data/helpdesk/attachments/production/155003147830/original/rZhxXwK1RQ8Y9Xv_B_alphp4o5jUgM8tzg.png?1689684933)
* Check if messaging is enabled.![](https://s3.amazonaws.com/cdn.freshdesk.com/data/helpdesk/attachments/production/155003147789/original/y8FWCdE6ybipFiVU89SU4W4hH-PmnWEZgA.png?1689684886)
* If the page is connected, but your IG page is still not visible as an option in your CRM. Please do a [hard reset](https://www.contractsafe.com/support/how-to-clear-your-browser-cache-and-hard-refresh) and then attempt to connect.

### **Messenger/ Instagram not syncing all messages:**

Sometimes the reason for this issue is our LeadConnector app is not set as the primary receiver if they have multiple CRM integration.

**Steps to resolve:**

* Switch to the desired FB page and [go to this link](https://www.facebook.com/settings?tab=advanced%5Fmessaging)![](https://s3.amazonaws.com/cdn.freshdesk.com/data/helpdesk/attachments/production/155003150048/original/T9EVwMfrAxqi2nsFwTXrAgUXjT7mjGC7WA.png?1689686311)![](https://s3.amazonaws.com/cdn.freshdesk.com/data/helpdesk/attachments/production/155003150854/original/I_uoXAcXds2D4qXFoXA652ovYkrEALHa9g.png?1689686853)

###   
**Leads, not syncing Issue:**

We need to check the business side for the places below.

* User Added to business(EMPLOYEE OR ADMIN)![](https://s3.amazonaws.com/cdn.freshdesk.com/data/helpdesk/attachments/production/155003151291/original/2Ywogek4UF9j2GkFpYjG6Dz0ucqzqqf1Nw.png?1689687116)
* FB Page Admin:![](https://s3.amazonaws.com/cdn.freshdesk.com/data/helpdesk/attachments/production/155003152796/original/XPUxQoPsF0M9oJsIzKiuM1CD131_iSXPvw.png?1689687942)
* Ad Account Check:  
   * Page Owner should Match with Ad Account Owner![](https://s3.amazonaws.com/cdn.freshdesk.com/data/helpdesk/attachments/production/155003152728/original/s14ryWLvkowGzFuNZfza4lH2mmIA7EG4eA.png?1689687921)
* Integration Lead Access Check:![](https://s3.amazonaws.com/cdn.freshdesk.com/data/helpdesk/attachments/production/155003152862/original/uEsoqFzJz0sF0XjS-b9Hum6FzZVah84wYw.png?1689687986)![](https://s3.amazonaws.com/cdn.freshdesk.com/data/helpdesk/attachments/production/155003152693/original/Uzc-o4zovZeYGG8TOMFpCNCvE2Kta27_wA.png?1689687900)  
   * If you are still not receiving the leads. Click on `**Restore Default Access**` it and check it again.

### **How to connect Instagram Account to the FB page or verify it is connected:**

An Instagram account can be connected to a single FB page.

Steps to connect the Instagram page or verify it is connected to the correct FB page 

  
Log in to Facebook and click **Pages** in the left menu.  
![](https://s3.amazonaws.com/cdn.freshdesk.com/data/helpdesk/attachments/production/155003153232/original/85dJI-K0071R82p4bCWUGkop8YrGGPwYPA.jpeg?1689688246) 

1. Select your Facebook page(Switch to the FB page), then click **Settings**![](https://s3.amazonaws.com/cdn.freshdesk.com/data/helpdesk/attachments/production/155003153563/original/-vhpzQAelDOYqi_G-4qjoueOWHwvvVI6kA.png?1689688414)  
Select **Linked Accounts** in the left column.  
Select **Instagram**, then connect your account.  
If it is already connected, we can verify this.  
    
![](https://s3.amazonaws.com/cdn.freshdesk.com/data/helpdesk/attachments/production/155003153740/original/N1GAJSmayrCpvMH1Au0XLVR269ZCdeLBMw.png?1689688510)  
    
If it is not connected. It will show like below![](https://s3.amazonaws.com/cdn.freshdesk.com/data/helpdesk/attachments/production/155003144114/original/foHC1Kh2bxUMx7_CKIUDUJxYGuYgNwRGQw.jpeg?1689682988)

**Pages Missing**

  
If an admin of a page also has their business account associated with the same page, they won’t be able to see the page while integrating with HighLevel. The best workaround is to add a second admin to that Facebook page, and have them integrate. Steps to add an admin to the page:

* Log in to Facebook and click on your profile photo in the top right corner.
* Select “See all profiles” and choose the Page you want to grant access to.
* Click the profile picture of your Page in the top right to navigate to your Page.
* Click “Manage,” then select “Page access” on the left under “Your tools.”
* Next to “People with Facebook access,” click “Add New.”
* Click “Next,” and then enter the name or email address of the person you want to grant Facebook access to. Finally, click on their name.
* You can now choose to grant either partial or full control over the Page:  
   * For partial control, scroll down and click “Give Access.”  
   * For full control, scroll down, click to grant full control, and then click “Give Access.”
* Type in your Facebook password to confirm the action, then click “Confirm.”
* The person you’ve granted access to will receive an email invitation to accept your invitation to access the Page.

  
By following these steps, we’ll successfully grant admin access to the user who will be connecting the Facebook account from GHL. This will allow them to manage the Page in the new Pages experience. After granting the admin access to the user, they would be able to successfully add the Facebook page to GHL.

  
This is temporary, we are working with Meta to get this fixed, reported here <https://developers.facebook.com/community/threads/712197940934624/>