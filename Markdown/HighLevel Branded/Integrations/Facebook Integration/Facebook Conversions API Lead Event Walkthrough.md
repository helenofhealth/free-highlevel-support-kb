**Date Updated:** 2025-06-11T12:10:33.000Z

### 

Facebook Conversions API aims to connect your marketing data directly with Funnels and Workflows in LeadConnector and Facebook Meta that help optimize ad targeting, decrease cost per result, and measure outcomes. With Facebook Conversion API, you can collect the people who are more likely relevant audiences for running your ads for retargeting. It is a setup for your business to upload server events for your web traffic. 

  
#### **Covered in this Article**

#### [**What is the difference between Funnel Events and Lead Events in Facebook Conversion API?**](#What-is-the-difference-between-Funnel-Events-and-Lead-Events-in-Facebook-Conversion-API?)

#### [**How to set up FB CAPI (Conversions API) Lead Event?**](#How-to-set-up-FB-CAPI-%28Conversions-API%29-Lead-Event?)

#### [Step 1: Create an FB Pixel:](#Step-1%3A-Create-an-FB-Pixel%3A)

#### [Step 2: Create two FB Conversions API Workflows.](#Step-2%3A-Create-two-FB-Conversions-API-Workflows.)

#### [Workflow -1 to Create/Update Opportunity](#Workflow--1-to-Create/Update-Opportunity)

#### [Workflow -2 to send Conversion data to FB Conversion API](#Workflow--2-to-send-Conversion-data-to-FB-Conversion-API)

---

## **What is the difference between Funnel Events and Lead Events in Facebook Conversion API?**

  
In LeadConnector, we support two types of Facebook Conversion API. 

  
**Funnel Events** \- 

The events are sent from a web server to record the events when the user visits the page, adds products to a cart, purchase, subscribe, submit an application, and more. To learn more about how to set up Funnel Event Pixel using FB CAPI, [please read this article.](https://help.gohighlevel.com/support/solutions/articles/48001236281-how-to-set-up-a-funnel-event-pixel-for-facebook-conversion-api-)

  
**Lead Events** \- 

The LeadConnector CRM sends the events with how the Lead moves across the pipeline stages. For example, a Business creates a pipeline name Lead Generation. The leads are moving across the pipeline stages, from new leads to booked or abandoned ones. With Lead events, LeadConnector CRM sends the data to Facebook Conversion API - with CRM being the data source. 

  
**Conversion Leads -** 

Facebook conversion leads integration helps your Facebook lead ads Instant Forms optimize for the quality of leads instead of the volume of leads. When users submit the Instant form, their contact information is captured and synced in Highlevel's CRM. This contact information can then be used to follow up with the leads to nurture them and move them further down the sales funnel. As each Lead moves through the sales funnel, the Conversion leads integration allows the advertiser to share the lead status with Meta, which allows Meta to optimize the lead ad for increased lead-to-sales Conversion. will enable
  
  
Guidelines to ensure your business is a good fit for the Conversion Leads integration:

* Use Facebook/Instagram Lead Ads (Instant Forms) \[Facebook form field mapping inside LeadConnector is used\]
* Ensure the 15-16 digit Meta Lead ID is mapped to your CRM
* Generate at least 250 leads per month
* Can upload data regularly at least once per day
* The lead stage you want to optimize for occurs within 28 days of leads being generated
* The lead stage you want to optimize for has a 1% - 40% conversion rate.

##   

---

## **How to set up FB CAPI (Conversions API) Lead Event?**

### **Step 1: Create an FB Pixel:**

  
1. Please start creating a pixel by going to your [Facebook Business Manager (also called the Meta Business Suite)](http://business.facebook.com) \> Head over to the left and then the **[Events Manager](https://www.facebook.com/events%5Fmanager2/)** tab.
2. Ensure you are connected to the correct Ad Account with all the required Access to that FB Page.  
![](https://s3.amazonaws.com/cdn.freshdesk.com/data/helpdesk/attachments/production/48284070737/original/AFb9bOXlqhbRRlui5ZOjvh_Ry7MYiUeFaQ.png?1677521079)
3. Head over to the left sidebar and then click on **Connect Data Sources![](https://s3.amazonaws.com/cdn.freshdesk.com/data/helpdesk/attachments/production/48284518426/original/vpJQuXlQ-fkLtQlkuMXpv-MYw6ymdVS3Ug.png?1677678141)**
4. Choose **CRM** in the options that show up, and then click on **Next.**![](https://s3.amazonaws.com/cdn.freshdesk.com/data/helpdesk/attachments/production/155031417908/original/SXjzS115ZEI927ZTXt0zAvEI0bBuEcBLCQ.png?1724240865)
5. It will show you a popup with Best Practices and a button to click **Next.** The Best Practices are Facebook suggestions on how to utilize this capability best. Click on **Next** to proceed.**![](https://s3.amazonaws.com/cdn.freshdesk.com/data/helpdesk/attachments/production/155031418022/original/D_jziC5xhCpZoJCvvQpjoKo3oRcKqijDJA.png?1724240955)**
6. Click on **Create New Pixel** or Use an existing pixel from the list for collecting the data. Click **Continue** when the pixel details are added.![](https://s3.amazonaws.com/cdn.freshdesk.com/data/helpdesk/attachments/production/48284072690/original/qgMYOqAYudCL0t2rtYthWAkL4dYkgKtGTw.png?1677521908)
7. After creating or selecting the pixel. Choose "LeadConnector" as CRM partner and click on **Next**![](https://s3.amazonaws.com/cdn.freshdesk.com/data/helpdesk/attachments/production/155031418374/original/hp1Pm_bswB-zDAdXVebjn_6oA1HL4dFSQA.png?1724241213)  
**Note:**  
Once you click on **Next**, Facebook redirects you to login to the partner website, one can ignore that and go ahead with creating a Conversion API workflow to send back CAPI events to Facebook.
8. You will see the below screen where your CRM is selected.  
**Important Note:** If you are facing the issue of being stuck at "Wait for seven days of CRM events" make sure to -  
# Send the data daily (consistently) to your pixel  
# Make sure that the count of events adds up to at-least 50 events for 7 days.  
# No test events will be considered as actual events  
# Atleast 2 stages in your pixel should have the pixel events
9. **![](https://s3.amazonaws.com/cdn.freshdesk.com/data/helpdesk/attachments/production/155031418496/original/e5AHKLIef3hvMEb0cA9Rk8nM8DFhCPYTGg.png?1724241315)**
10. Now you can start sending CRM events for which you will need to setup two workflows which is explained below.

  
**Please Note**

**Prerequisite for Facebook CAPI - Lead Events**  
1. In CRM, please go to Settings > Integration > Check the Facebook account is connected with admin permissions. Please ensure that your FB Business Page, which you are an admin of and have all access to, [is integrated and the correct FB lead Form is mapped in your CRM account.](https://help.gohighlevel.com/support/solutions/articles/48000987779-facebook-lead-ad-integration-troubleshooting-guide)  
![](https://s3.amazonaws.com/cdn.freshdesk.com/data/helpdesk/attachments/production/155031419137/original/NyIl9s0xM-cgct_0BaT_tihv76t_6-bsDA.png?1724241655) ![](https://s3.amazonaws.com/cdn.freshdesk.com/data/helpdesk/attachments/production/155031419242/original/Kv8uEaz2OIhtlVC7pRQJrvQmyXjX4DliLw.png?1724241732)2. In Facebook From Field Mapping, the form should be mapped correctly and the status should be enabled. Facebook form mapping has moved under location settings > integrations > Facebook Form Field Mapping. [Here is a list of the supported custom fields](https://help.gohighlevel.com/support/solutions/articles/48000987779-facebook-lead-ad-integration-troubleshooting-guide#Supported-custom-fields-when-using-Facebook-Lead-Ads%3A) which include multiple and single option custom fields as well.  
  
![](https://s3.amazonaws.com/cdn.freshdesk.com/data/helpdesk/attachments/production/48289200906/original/NguctF2neILw1L4MOJy_0UMZ_hv_wBTooA.gif?1679678976)[](https://help.gohighlevel.com/support/solutions/articles/48000987779-facebook-lead-ad-integration-troubleshooting-guide#Supported-custom-fields-when-using-Facebook-Lead-Ads%3A:~:text=Facebook%20form%20mapping%20has%20moved%20under%20location%20settings%20%3E%20integrations%20%3E%20Facebook%20Form%20Field%20Mapping)![](https://s3.amazonaws.com/cdn.freshdesk.com/data/helpdesk/attachments/production/48286543798/original/TN-M497JjRU1QI1H-NwXVq1r1vWxdBHPWw.png?1678462304)

  
### **Step 2: Create two FB Conversions API Workflows.**

  
**Please Note**

**You need to create Two Workflows for this process to work effectively.**  
  
The first workflow focuses on generating leads and adding them to the correct pipeline with an **Create/Update Opportunity Action**. Once a lead is captured, it is important to ensure that it is properly tagged and categorized in the correct Pipeline and Stage so that it can be effectively managed and tracked as it moves through your sales funnel.  
  
The second workflow focuses on triggering events for Facebook conversion leads. The goal of this workflow is to get fired off by a lead being moved to a specific pipeline stage and then a Facebook Conversions API workflow action pushes them to FB CAPI.  
  
By combining these two workflows, you can create a comprehensive lead generation and management system that is optimized for Facebook conversion leads. This can help you generate more qualified leads, convert more customers, and grow your business over time.

  
To send a CRM event from your CRM, you need to create a workflow that does that. For now, you can navigate away from the **FB Events Manager> Data Sources> Settings (but keep it open in a tab in your browser)**and head over to your CRM account.

#### ![](https://s3.amazonaws.com/cdn.freshdesk.com/data/helpdesk/attachments/production/48284081045/original/r6dBGPrK4R-SDzJJARAeMGvHU6SwuwwTog.png?1677525316)  
**Workflow -1 to Create/Update Opportunity**

####   

1. Once the FB page is integrated correctly in sub-account settings, go to your **Automations> Workflows** **\>Create a new Workflow.![](https://s3.amazonaws.com/cdn.freshdesk.com/data/helpdesk/attachments/production/155031420060/original/KGiogaGqC8eiladKNdMI3LxVnUoi6nqgcw.jpeg?1724242169)**
2. **Add a new Workflow Trigger** in your Workflow and have it get fired off by **Facebook Lead Form Submitted** (if that is the first stage of your conversions flow)![](https://s3.amazonaws.com/cdn.freshdesk.com/data/helpdesk/attachments/production/155031420109/original/VmYgHXIBM5dLZ6_u8p9Q79sQ15kbzgBwIQ.jpeg?1724242198)
3. You can add filters to choose which specific Facebook Lead Ad form to get the Workflow to be triggered by submissions to that form only![](https://s3.amazonaws.com/cdn.freshdesk.com/data/helpdesk/attachments/production/155031420115/original/_Bhbh1Hc2u_baOSGlOZEe7ucGSdUnvUcDw.jpeg?1724242216)
4. After this, add another action for **"Facebook Conversion API". ![](https://s3.amazonaws.com/cdn.freshdesk.com/data/helpdesk/attachments/production/155024366350/original/hX8DzXO3Ka_6YyRNN5DBviUV6nhfevSOiA.png?1712915506)**
5. Add the required details for Access Token, Pixel ID and Stage Name. **![](https://s3.amazonaws.com/cdn.freshdesk.com/data/helpdesk/attachments/production/155024366296/original/RKorAYSA0fWsEKXs_UNljAG1MBfV48vukQ.png?1712915461)**  
    
    
**Note:**  
**Addition of Custom Values -**  
Similar to Google Ads, we are now allowing custom mapping for Facebook Ads conversion tracking parameters.  
    
    
![](https://s3.amazonaws.com/cdn.freshdesk.com/data/helpdesk/attachments/production/155043836459/original/gFVWuYxc77LoQwMEWkY0p_spdSoyA3QWZQ.jpeg?1742815441)  
    
    
**How It Works:**  
    
By default, custom mapping is disabled.  
Users can toggle it on to enable custom mapping.  
    
When enabled, users can map:  
1. FBCLID for funnel events.  
2. Facebook Lead ID for lead events.  
3. If custom mapping fields are provided, they will take priority over system defaults.  
4. If left empty, the system will continue using its default internal values.
6. For the Access Token, head over to your **Facebook Events Manager> Data Sources> Settings> Scroll down and click on Generate Access Token.** Once generated copy the Access token and paste it in the workflow action configuration.![](https://s3.amazonaws.com/cdn.freshdesk.com/data/helpdesk/attachments/production/155031421996/original/2M5kyzuzDEJFC4zHnrjdGIF4Hld8a-cnrw.png?1724243441)
7. For the Pixel ID, head over to your **Facebook Events Manager> Data Sources> Settings> Scroll down and copy your Dataset ID** (this will be Pixel ID). Paste the **Pixel ID** in the **Pixel ID** field in your Workflow's **FB Conversion API Action.**  
**![](https://s3.amazonaws.com/cdn.freshdesk.com/data/helpdesk/attachments/production/155031422924/original/u9buQQXLzvtO596soAHgCdul47lg-Q2B0Q.jpeg?1724243971)**
8. And then add the action for Create or Update Opportunity. Also specify the Pipeline and Pipeline Stage for this action.![](https://s3.amazonaws.com/cdn.freshdesk.com/data/helpdesk/attachments/production/155024366504/original/IVGX9z5k0pWkkpq_kMQOJOuJv-C-jRZgWg.png?1712915642)
9. The Opportunity Name can be defaulted to the Lead's Full Name by using the custom value dropper:![](https://s3.amazonaws.com/cdn.freshdesk.com/data/helpdesk/attachments/production/155031420481/original/naZd6SFqXIQhb2IxIgUICHcWTVws3FuGIA.png?1724242432)
10. Toggle on Allow Duplicate Opportunities for this particular Workflow.![](https://s3.amazonaws.com/cdn.freshdesk.com/data/helpdesk/attachments/production/155031420583/original/tRcVgVuLqAga6QSyFl1xphZT2y43y33LSw.png?1724242482)
11. Publish and Save the workflow

####   
  
**Workflow -2 to send Conversion data to FB Conversion API**

####   

1. #### Create another workflow. Add the **Pipeline Stage Change** trigger and a **Facebook Conversion API** action.  
![](https://s3.amazonaws.com/cdn.freshdesk.com/data/helpdesk/attachments/production/155031421020/original/23qX6oljE-grIUfBMMkiXCy7bEISawvVAA.png?1724242774)
2. #### Choose **Lead Event** as the **Event Type.** Enter the**Access Token** and **Pixel ID**.  
For **Stage Name** : It should accurately represent your Pipeline and Pipeline Stage name for better reporting. Select it using the tag icon at the end to add the custom value of the opportunity pipeline and stages. ![](https://s3.amazonaws.com/cdn.freshdesk.com/data/helpdesk/attachments/production/155031421279/original/6zhHzNBl6SBJA4I4Ka6hqh6TUBvTEap9Yw.png?1724242985)
3. #### For the Access Token, head over to your **Facebook Events Manager> Data Sources> Settings> Scroll down and click on Generate Access Token.** Once generated copy the Access token and paste it in the workflow action configuration.![](https://s3.amazonaws.com/cdn.freshdesk.com/data/helpdesk/attachments/production/155031421996/original/2M5kyzuzDEJFC4zHnrjdGIF4Hld8a-cnrw.png?1724243441)
4. For the Pixel ID, head over to your **Facebook Events Manager> Data Sources> Settings> Scroll down and copy your Dataset ID** (this will be Pixel ID). Paste the **Pixel ID** in the **Pixel ID** field in your Workflow's **FB Conversion API Action. ![](https://s3.amazonaws.com/cdn.freshdesk.com/data/helpdesk/attachments/production/155031422219/original/GziRBRRy5Z7j0_VsRySWWjl4FnVx6E3FQg.png?1724243552)**
5. Save the Action, **Save** and **Publish** the Workflow.
6. You can test your Workflow using the [Lead Ads Test Tool.](https://developers.facebook.com/tools/lead-ads-testing) Choose the correct Page and Lead Ad Form, then **Create a Lead.**  
**![](https://s3.amazonaws.com/cdn.freshdesk.com/data/helpdesk/attachments/production/155031422501/original/4Sqw2Xl0VmEdLphpxjo61cpNXWF1ETpf1w.png?1724243742)**
7. The Event should be picked up by your Events Manager, which is actively waiting for Events sent by your Workflow. It takes up to a day to successfully pick up an event sent by your Workflow.
8. Once the Event is sent from the Lead Ads Test Tool, please go to Opportunity Pipeline and move the dummy Facebook lead to another stage configured in the Workflow. Once this is completed, check the workflow status as executed and the conversion API event in Event Manager.  
    
![](https://s3.amazonaws.com/cdn.freshdesk.com/data/helpdesk/attachments/production/48289807416/original/lPWKPzVG8LSj7hT4URdCTXBJsQAya3ue-Q.png?1680028394)
  
  
11\. Return to the “settings” tab in Events Manager to track the progress of the Conversion Leads integration. 
  
  
**Important Note** - For both the above worflows, please enable **Allow Multiple** in Workflow Settings.  
  
![](https://s3.amazonaws.com/cdn.freshdesk.com/data/helpdesk/attachments/production/48284914523/original/l_2ib3vbuisvYM3kwkrFC6fJvfGmEAxTiA.jpeg?1677797816)
  
  