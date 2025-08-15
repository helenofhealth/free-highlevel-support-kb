**Date Updated:** 2022-09-19T20:26:12.000Z

Facebook Ads are a great way to promote your business, but you need to make sure that they’re set up correctly. If you don’t have the right settings in place, then it could be costing you money and wasting time.

  
In this article, we’ll show you how to check your Facebook ad setup so you can get the most out of them.
  
  
**Covered in this article:**

#### [**How to troubleshoot your Facebook Ad Reporting setup:**](#How-to-troubleshoot-your-Facebook-Ad-Reporting-setup%3A)

[1\. The Integration of the Facebook Ad Account needs to be active](#1.-The-Integration-of-the-Facebook-Ad-Account-needs-to-be-active)

[2\. UTM Tracking template should be added at Tracking, not at the Destination.](#2.-UTM-Tracking-template-should-be-added-at-Tracking,-not-at-the-Destination.)

[3\. The uniqueness of the Name for the Facebook Ads, Ad-set, and Campaign is necessary.](#3.-The-uniqueness-of-Name-for-the-Facebook-Ads,-Ad-set-and-Campaign-is-necessary.)

[4\. Changing Facebook ad campaigns, Ad-sets, and ads won't affect the copy of UTM’s side of Facebook Ads. They attribute to old parameters.](#4.-Changing-Facebook-ad-campaigns,-Ad-sets-and-ads-won't-affect-the-copy-of-UTM%E2%80%99s-side-of-Facebook-Ads.-They-attribute-to-old-parameters.)

[5\. While connecting Facebook Lead Form Mapping, it is necessary to choose the correct Facebook Page.](#5.-While-connecting-Facebook-Lead-Form-Mapping,-it-is-necessary-to-choose-the-correct-Facebook-Page.)

  
---

## **How to troubleshoot your Facebook Ad Reporting setup:**

  
### **1\. The Integration of the Facebook Ad Account needs to be active**

  
It is necessary to check that the Facebook Ad Account connected in sub-account > settings > integrations[ has admin permissions.](https://web.facebook.com/business/help/1588743581429919?id=735435806665862&%5Frdc=1&%5Frdr#:~:text=Note%20that%20you%20must%20be%20an%20admin%20of%20the%20Facebook%20Page%20and%20have%20leads%20access%20permissions%20in%20order%20to%20connect%20a%20CRM%20system.)

  
**Please Note:**

Not seeing your page on the integration section of the CRM. Please check out - [How to assign crm access](https://web.facebook.com/business/help/1588743581429919?id=735435806665862&%5Frdc=1&%5Frdr#:~:text=Note%20that%20you%20must%20be%20an%20admin%20of%20the%20Facebook%20Page%20and%20have%20leads%20access%20permissions%20in%20order%20to%20connect%20a%20CRM%20system.)  
   
[If you are in fact the FB Admin, can you try this to confirm if Lead Connector is accessible and can allow access to your page?](https://help.gohighlevel.com/support/solutions/articles/48000987779-facebook-lead-ad-integration#:~:text=If%20are%20in%20fact%20the%20FB%20Admin%2C%20can%20you%20try%20this%20to%20confirm%20if%20Lead%20Connector%20is%20accessible%20and%20can%20allow%20access%20to%20your%20page%3F)
  
  
To advertise for a Facebook Page and Instagram account in Meta Ads Manager, you need to do the following:  
  
Advertising accounts have 3 types of admin permissions available to help you manage your account. When you give someone permission to access your ad account, you choose what they're able to do or see by assigning them a role. The table below outlines the 3 ad account roles (across) and what they're able to do (down):  
  
![](https://s3.amazonaws.com/cdn.freshdesk.com/data/helpdesk/attachments/production/48248640131/original/i4b0NyjU-xcO7XDQpNq_pAs_KhnqHRGR3Q.png?1662042909)  
**Please Note:**

You need to be a Page admin or ask a Page admin to [assign you a Page admin (recommended), editor, moderator, advertiser or jobs manager role. ](https://www.facebook.com/help/187316341316631?helpref=faq%5Fcontent)Note: If you have transitioned to the [new Pages experience and have task access](https://www.facebook.com/business/help/1101781386943864), you can manage ads from Ads Manager or Meta Business Suite.
  
  
###   
**2\. UTM Tracking template should be added at Tracking, not at the Destination.**

Additional resources - [How to set up Facebook Ad Reporting](https://help.gohighlevel.com/en/support/solutions/articles/48001204042)[](https://help.gohighlevel.com/en/support/solutions/articles/48001204042)**[](https://help.gohighlevel.com/en/support/solutions/articles/48001204042)**

  
![](https://s3.amazonaws.com/cdn.freshdesk.com/data/helpdesk/attachments/production/48247908119/original/hfjpXumheRhCLWFfZsAOubs4t7ZjtSS_Lw.jpeg?1661784949)

  
###   
  
**3\. The uniqueness of the Name for the Facebook Ads, Ad-set, and Campaign is necessary.**

If the names are not unique, it will show duplicate entries of contacts in different ad-set/Ad in Facebook Ad.  
  
**What not to do:**

  
| **Campaign Name** | New Restaurant in Town |
| ----------------- | ---------------------- |
| **Campaign id**   | 12345                  |
| **Ad Set**        | Dish 1                 |
| **Ad**            | Fresh Red Pasta        |
| Dish 2            |                        |
| **Ad**            | Fresh Red Pasta        |

  
In this example, Customer A gets created with Paid Search. Customer A will be present in the Leads column of Facebook Ad Reporting in Ad named as Nike Sport Shoes 1 in two different ad-sets.  
  
https//example.com?utm\_source=fb\_ad&utm\_medium={dish1}&utm\_campaign={newrestaurantintown}&utm\_content={freshredpasta}&campaign\_id={12345}
  
  
**Correct Setup:**  
  
| **Campaign Name**  | New Restaurant in Town               |
| ------------------ | ------------------------------------ |
| **Campaign id**    | 12345                                |
| **Ad Set**         | Dish 1 Starter                       |
| **Ad**             | 1.1 Fresh Red Pasta with extra sauce |
| Dish 2 Main Course |                                      |
| **Ad**             | 2.1 Fresh Red Pasta with no sauce    |

  
###   
  
  
**4\. If you change the name of the Facebook ad campaigns, Ad-sets, and ads it won't affect the copy of UTM’s side of Facebook Ads. They attribute to old parameters.**

We would recommend creating new Campaigns, Ad-sets, and Ads. The list view of Facebook Ad Reporting in the CRM will update the name but the data will stop attributing sales, leads, and ROI as UTMs are still associated with the old Campaigns, Ad-sets, and Ads.

* The name parameters can’t be changed during the lifetime of the campaign / Ad-set / Ad. If the name has to be changed, then create a different campaign / Ad-set / Ad.
* If you decide to change the name of the campaign / Ad-set / Ad but you do NOT create a new campaign, then the data in the CRM system will keep referring to the original/ first campaign. \[Facebook Ad provides the old name in the parameter\]
  
  
### **5\. While connecting [Facebook Lead Form Mapping](https://help.gohighlevel.com/support/solutions/articles/48000987779-facebook-lead-ad-integration#:~:text=Facebook%20form%20mapping%20has%20moved%20under%20location%20settings%20%3E%20integrations%20%3E%20Facebook%20Form%20Field%20Mapping), it is necessary to choose the correct Facebook Page.**

  
It is necessary to map as active to collect the Facebook forms leads.

  
**Please Note:**

Text fields along with custom fields can be mapped up easily.  
Radio custom fields cannot be mapped with Facebook Lead forms  
You will not be able to map a Timezone field.
  
  