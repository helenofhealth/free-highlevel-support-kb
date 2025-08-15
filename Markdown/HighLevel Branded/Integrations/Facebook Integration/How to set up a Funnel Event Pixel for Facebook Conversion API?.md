**Date Updated:** 2025-03-24T16:49:24.000Z

Facebook Conversions API (or CAPI) is designed to help businesses deliver personalized advertising experiences to customers and audiences, all while maintaining data privacy. This tool lets you send web events directly to Facebook from their respective servers. If you use a Facebook Pixel to track events for your ads, you will want to add the Pixel code to your funnel and funnel steps.

  
#### **Covered in this Article:**

#### [**How to set up FB CAPI (Conversions API) Funnel Event?**](#How-to-set-up-FB-CAPI-%28Conversions-API%29-Funnel-Event?)

#### [Step 1: Create an FB Pixel:](#Step-1%3A-Create-an-FB-Pixel%3A)

#### [Step 2: Apply Pixel Code to your Funnel/Website.](#Step-2%3A-Apply-Pixel-Code-to-your-Funnel/Website.)

#### [Step 3: Create a Facebook Conversions API Workflow.](#Step-3%3A-Create-a-Facebook-Conversions-API-Workflow.)
  
  
---

## **How to set up FB CAPI (Conversions API) Funnel Event?**

### **Step 1: Create an FB Pixel:**

  
1. Please start creating a pixel by going to your [Facebook Business Manager (also called the Meta Business Suite)](http://business.facebook.com) \> Head over to the left and then the **[Events Manager](https://www.facebook.com/events%5Fmanager2/)** tab.
2. Ensure you are connected to the correct Ad Account with all the required Access to that FB Page.  
![](https://s3.amazonaws.com/cdn.freshdesk.com/data/helpdesk/attachments/production/48284070737/original/AFb9bOXlqhbRRlui5ZOjvh_Ry7MYiUeFaQ.png?1677521079)
3. Head over to the left sidebar and then click on **Connect Data Sources![](https://s3.amazonaws.com/cdn.freshdesk.com/data/helpdesk/attachments/production/48284518426/original/vpJQuXlQ-fkLtQlkuMXpv-MYw6ymdVS3Ug.png?1677678141)**
4. Choose **Web** in the options that show up, and then click on next**.**  
![](https://s3.amazonaws.com/cdn.freshdesk.com/data/helpdesk/attachments/production/155031423162/original/o_ZF2cyQyA9qLqbmCcAB4FnSrMwgM_mZVA.png?1724244130)
5. If you already have pixels, it will ask you to choose between them or create a new pixel. Click on **Create new Pixel** or Use an existing pixel from the list for collecting the data. Click **Continue** when the pixel details are added.![](https://s3.amazonaws.com/cdn.freshdesk.com/data/helpdesk/attachments/production/48284072690/original/qgMYOqAYudCL0t2rtYthWAkL4dYkgKtGTw.png?1677521908)![](https://s3.amazonaws.com/cdn.freshdesk.com/data/helpdesk/attachments/production/48289558054/original/bJeFGIeh-ZoGTd2Tb-3fON8lBJOKZVrzmw.png?1679940937)
6. It will then ask you to provide the URL of the CRM's website/funnel where you will add your pixel code.  
![](https://s3.amazonaws.com/cdn.freshdesk.com/data/helpdesk/attachments/production/48289558739/original/PAF__5OhEXarHQx5f1VRZQ0TZlm-vIbsgw.png?1679941181)
7. Please add in the domain of the funnel/website where you will later add in the pixel code and then click on **Check.** If your domain is eligible for this process, then you will see a green checkmark in the domain field. Once you see the green checkmark, click on the **Next** button that appears instead of the **Check** button.![](https://s3.amazonaws.com/cdn.freshdesk.com/data/helpdesk/attachments/production/155031423710/original/veyxXsSA6Fng_0nJJ-h34zDLk_G0T6pHwg.png?1724244460)
8. It will then show you a popup asking you to **Choose how to connect your website.** Choose the first option, **Meta Pixel and Conversions API.![](https://s3.amazonaws.com/cdn.freshdesk.com/data/helpdesk/attachments/production/155031423772/original/2XKJ_iM3ak-QJYnGV9iaEabCoJ7BRz3YrQ.png?1724244493)**
9. After this you will be see the Instructions. Click on "See Instructions" under Conversions API **![](https://s3.amazonaws.com/cdn.freshdesk.com/data/helpdesk/attachments/production/155031423901/original/XVw12VjtzU_VoAP_6bxCjCNv6rLP6dILvA.png?1724244584)**
10. It will take you to the **Overview** tab for the **Manual Implementation** process. Read through the instructions and then click on **Continue.![](https://s3.amazonaws.com/cdn.freshdesk.com/data/helpdesk/attachments/production/155031424024/original/hiVjRqpxZCO_lViZiYsnTLm4ZXEmVGnAzA.png?1724244660)**
11. You will then be taken to the **Select Events** tab. You will see a dropdown to choose which Industry you are setting up this Pixel for. Choose the one most relevant to your client.![](https://s3.amazonaws.com/cdn.freshdesk.com/data/helpdesk/attachments/production/155031424282/original/nM0VnSjCU1DEyuvCgbr5GGwT6QoDPYGu5g.png?1724244784)
12. Then it would be best to choose the events you want to send to Facebook. Select all the events you wish to send to Facebook, and click on **Continue**.![](https://s3.amazonaws.com/cdn.freshdesk.com/data/helpdesk/attachments/production/155031424238/original/CRl1a7eHHek535QvXq7QhCP5BFmrWYaPkg.png?1724244768)
13. You will be taken to the **Select Parameters** tab, where a few **Event Detail Parameters** will already be checked. Checkmark **Event ID,** as the Best Practices tooltip recommends it to the right.![](https://s3.amazonaws.com/cdn.freshdesk.com/data/helpdesk/attachments/production/155031424309/original/CHbZI63v1OjLOi_Ha7h6oHqyfTj0LVvOuQ.png?1724244811)![](https://s3.amazonaws.com/cdn.freshdesk.com/data/helpdesk/attachments/production/155031424379/original/McMYaiuIvhk2Q6px-7hY3s_a_EaRqfbWJA.png?1724244863)
14. Then, under **Customer Information Parameters**, you will see that **Client User Agent** will already be marked for you. You must check the **Client's IP Address, First Name, Client ID, Email, Business ID, and Last Name. (IMP NOTE -**You need to at-least select the same checkboxes for every single event that you added to this Pixel.)  
![](https://s3.amazonaws.com/cdn.freshdesk.com/data/helpdesk/attachments/production/155031424583/original/FeAiafdKndcnOzPuYaRsELSlYdmsKUSQqw.png?1724244990)
15. It will then ask you to **review the Setup** and check all the Parameters you have chosen for each **Event one last time.** Once you are sure everything is set up as you need it to be, click on **Continue![](https://s3.amazonaws.com/cdn.freshdesk.com/data/helpdesk/attachments/production/155031424785/original/WeAtZHPMuprCiu9Ut7Rm-FXrPifGfMrvhQ.jpeg?1724245080)**
16. In the next step, click on **Finish.**  
**![](https://s3.amazonaws.com/cdn.freshdesk.com/data/helpdesk/attachments/production/155031424804/original/ZF7ymYlO_hwJVYNgOe1F70jwjVg4FoAolA.png?1724245108)**
17. Now we will configure the browser pixel event. Select "Set up Meta Pixel".![](https://s3.amazonaws.com/cdn.freshdesk.com/data/helpdesk/attachments/production/155032148487/original/18Tq2VZt6EEZr6XOi9J4hVWjJlR_INnAeg.png?1725362743)
18. You will be shown a popup to **Connect website activity using Pixel; choose** **Install Code Manually**.![](https://s3.amazonaws.com/cdn.freshdesk.com/data/helpdesk/attachments/production/155032148583/original/-1I2AK9MpfruM7VYj8molxfqlhrpJF4FrA.png?1725362799)
19. Click on "Copy Code" to copy the meta pixel code![](https://s3.amazonaws.com/cdn.freshdesk.com/data/helpdesk/attachments/production/155032148600/original/OrLfiaNSvaZ4Bc4xMlmbiSB-rwcPXZa2VQ.png?1725362818)

###   

###   

## **Step 2: Apply Pixel Code to your Funnel/Website.**

1. Keep this browser tab open and navigate to your CRM account. Navigate to the **Sub** **Account** that you are setting up this Pixel for.
2. Head on to **Sites** in the left sidebar and then to **Funnels or Websites** (depending on where you built the site, which is associated with the domain you used in your Pixel Setup)![](https://s3.amazonaws.com/cdn.freshdesk.com/data/helpdesk/attachments/production/155032148908/original/7GdEB-pnC5XOcG6GQavHzbCNRMzbKgf-Wg.png?1725362991)
3. If you want to track on a specific page or step then, click on **Edit** and then preferably **Edit in a new tab** to open the Funnel Builder.**![](https://s3.amazonaws.com/cdn.freshdesk.com/data/helpdesk/attachments/production/155032149047/original/MeKMG4wy-FOm_6pRtYT2BZZbQU3NPfou_Q.png?1725363100)**
4. Once inside the builder, click on the code icon and paste the code you had copied previously in the "Header Tracking" section and then click on Save![](https://s3.amazonaws.com/cdn.freshdesk.com/data/helpdesk/attachments/production/155032149385/original/mEKP3Yv7hEmyp1blhUXtHd2fPdpq21S8wQ.png?1725363273)
5. If you want to track the Browser Event on all the pages or steps then you can do it by clicking on funnel or website settings and then pasting the code in the "Head tracking code" section![](https://s3.amazonaws.com/cdn.freshdesk.com/data/helpdesk/attachments/production/155032149705/original/-I69P-F4mIuQBcBpvAgRIT0QdTJSzLAnAA.png?1725363421)
6. Save your changes

###   
**Step 3: Create a Facebook Conversions API Workflow.**

1. Navigate to **Automation>Workflows>Create Workflow![](https://s3.amazonaws.com/cdn.freshdesk.com/data/helpdesk/attachments/production/155032150008/original/v-sU1upHoO-x9IGa4HLW6eW2dhwxPdAS4A.png?1725363584)**
2. Click on **Add New Workflow Trigger.** Here any of the following triggers can be used individually or in combination: Form Submitted, Customer Booked Appointment, Survey Submitted or Order Form Submission.**![](https://s3.amazonaws.com/cdn.freshdesk.com/data/helpdesk/attachments/production/155032150362/original/awZeptMVjJbwk_PPtS5jOvhQjl_kaXI21Q.png?1725363773)**
3. Once you have chosen the workflow trigger(s), you can add the filter to choose the specific form/calendar/order form/survey from where you want to track the pixel conversion events.
4. Then click on **Add your first Action.** Search for and select the **Facebook Conversion API** Action. Configure the **Facebook Conversion API** action. You can name this Action in **Action Name** if you'd like. In the **Event Type** dropdown, choose **Funnel Event.**  
![](https://s3.amazonaws.com/cdn.freshdesk.com/data/helpdesk/attachments/production/155032151023/original/XvIqeQ42GaEENsh1S-28AJ_RmIhxAx3aZw.png?1725364054)
5. For the Access Token, head over to your **Facebook Events Manager> Data Sources> Settings> Scroll down and click on Generate Access Token.** Once generated copy the Access token and paste it in the workflow action configuration.![](https://s3.amazonaws.com/cdn.freshdesk.com/data/helpdesk/attachments/production/155032151448/original/nNO1m9hBF53AoUjcdI6jTAngHwZjphesrg.jpeg?1725364264)
6. For the Pixel ID, head over to your **Facebook Events Manager> Data Sources> Settings> Scroll down and copy your Dataset ID** (this will be Pixel ID). Paste the **Pixel ID** in the **Pixel ID** field in your Workflow's **FB Conversion API Action.**  
**![](https://s3.amazonaws.com/cdn.freshdesk.com/data/helpdesk/attachments/production/155032151439/original/H-wRfkeISdeGz9XM_qxfxEA2gCQp8Ws5dQ.jpeg?1725364262)**
7. Paste the **Access Token and Pixel ID**  in the Facebook Conversion API Action's respected fields.![](https://s3.amazonaws.com/cdn.freshdesk.com/data/helpdesk/attachments/production/155032151572/original/bbgxCtJlb3G6T3FBXPaNEiouqGfy0gk1KQ.png?1725364339)
8. Once complete, **Save the Action** and then **Save** and **Publish** the Workflow.

  
**Please Note:**

**For Lead Value please use assumed values like 1000 or 2000 so that you can identify value each lead contributes to your pipeline.**

**![](https://s3.amazonaws.com/cdn.freshdesk.com/data/helpdesk/attachments/production/155032151876/original/WVpH1GiO1F91-z_v5JdN4YictKhz4kl3_g.png?1725364516)**
  
  
---

## **Custom Values:**

  
Similar to Google Ads, we are now allowing custom mapping for Facebook Ads conversion tracking parameters.

  
![](https://s3.amazonaws.com/cdn.freshdesk.com/data/helpdesk/attachments/production/155043835950/original/gG6WcLmyidLSEdiRgYprTlogL8BqVfs3aQ.png?1742815104)  

  
**How It Works:**

  
By default, custom mapping is disabled.

Users can toggle it on to enable custom mapping.

  
When enabled, users can map:

* FBCLID for funnel events.
* Facebook Lead ID for lead events.
* If custom mapping fields are provided, they will take priority over system defaults.
* If left empty, the system will continue using its default internal values.
  
  