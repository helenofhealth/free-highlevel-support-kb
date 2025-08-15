**Date Updated:** 2025-06-28T02:22:48.000Z
  
  
This Article is a complete guide for all cancellation processes for SaaS-enabled sub-accounts. It contains instructions on how to cancel a SAAS sub-account for your client and how to allow them to cancel their SAAS subscription with your Agency. 

  
**IMPORTANT**: Key points to remember when Cancelling Saas for a Sub-account.  
  
1. You must be logged in with an Agency-level (admin) user – sub-accounts can only be canceled by Agency admins.  
  
2. If you don’t see “Cancel SaaS” under Settings → SaaS, go to Agency Dashboard → Sub-accounts, click the three-dot menu on the client’s tile, and select “Cancel Subscription.”  
  
3. If the button is still missing, ensure the sub-account has an active SaaS plan. Inactive or trial accounts won’t show a cancel option.  
  
If you’ve verified the above and still can’t cancel, please reach out to HighLevel Support

---

**TABLE OF CONTENTS**

* [Instructions to cancel SaaS-enabled sub-account yourself](#Instructions-to-cancel-SaaS-enabled-sub-account-yourself)  
   * [Step 1: Reconcile SaaS Wallet Balance](#Step-1%3A-Reconcile-SaaS-Wallet-Balance)  
   * [Step 2: Disable SaaS on the Sub-Account from Agency View](#Step-2%3A-Disable-SaaS-on-the-Sub-Account-from-Agency-View)  
   * [Step 3: Close Twilio / Mailgun Sub-Accounts - For Clients who're leaving your Agency](#Step-3%3A-Close-Twilio-/-Mailgun-Sub-Accounts---For-Clients-who're-leaving-your-Agency)  
   * [Step 4: Remove User from Team Management / Delete the Sub-Account - For Clients who're leaving your Agency](#Step-4%3A-Remove-User-from-Team-Management-/-Delete-the-Sub-Account---For-Clients-who're-leaving-your-Agency)
* [Instructions to allow the client to cancel their subscription](#Instructions-to-allow-the-client-to-cancel-their-subscription)
* [FAQ](#FAQ)

---

## **Instructions to cancel SaaS-enabled sub-account yourself**

####   

### [**Step 1: Reconcile SaaS Wallet Balance**](https://help.gohighlevel.com/support/solutions/articles/48001207115-saas-wallet-credit-management#How-to-Remove-Credits-from-the-wallet?)

If the client has any non-complimentary credits in their wallet, you must refund those in Stripe.

You can check if the wallet credits are complimentary or non-complimentary by going to sub-account settings > Company Billing > See Details (Transaction History)

  
For more details, please review this article: [SaaS Wallet Credit Management ](https://help.gohighlevel.com/support/solutions/articles/48001207115-saas-wallet-credit-management)

  
![](https://s3.amazonaws.com/cdn.freshdesk.com/data/helpdesk/attachments/production/155048933937/original/xzJs8bQuXFcLRrINWXwPf49y7UohpaAqyg.png?1750947254)

---

### **Step 2: Disable SaaS on the Sub-Account from Agency View**

[](https://help.gohighlevel.com/support/solutions/articles/48001204857-ways-to-get-highlevel-support-24-7)Disable SaaS for this sub-account by going to Agency view > Accounts tab > View Details:

  
![](https://s3.amazonaws.com/cdn.freshdesk.com/data/helpdesk/attachments/production/155048932456/original/KsQf420juKKARMnRmEf2LjrBOwt9OSZLSw.png?1750946346)

  
Cancel the Stripe subscription if you no longer want to charge the client for the SaaS plan:

  
![](https://s3.amazonaws.com/cdn.freshdesk.com/data/helpdesk/attachments/production/155048934027/original/mYa8K1T3fvgB_AXmR-0r6W7eex-k19shKw.png?1750947323)

  
Note: We recommend exporting all transaction details before disabling SaaS, because once SaaS mode is disabled, all transaction/wallet history will be removed.

  
![](https://s3.amazonaws.com/cdn.freshdesk.com/data/helpdesk/attachments/production/155048934135/original/qhgKoztfS9gHywLjCb1XhDE-v-gYwhIIGA.png?1750947418)

---

### **Step 3: Close Twilio / Mailgun Sub-Accounts - For Clients who're leaving your Agency**

If the sub-account has Twilio or Email (Mailgun), Rebilling is turned on after disabling SaaS; their Twilio / Mailgun sub-account will still be connected in Agency Settings > Twilio / Mailgun. Make sure you've deleted those connections and closed these sub-accounts.  
  
  
---

### **Step 4: Remove User from Team Management / Delete the Sub-Account - For Clients who're leaving your Agency**

This step depends on your choice.

1. If you want to keep the client's data even after removing them, go to Agency Settings > Team and remove the client's user.
2. If you don't want to keep their data, go to Accounts > View Details, and delete the sub-account  
    
![](https://s3.amazonaws.com/cdn.freshdesk.com/data/helpdesk/attachments/production/48231582189/original/UNt-o4efJOfgcS8C_GZxKH-ffa-PJV6YAQ.png?1654802197)

---

## **Instructions to allow the client to cancel their subscription**

SaaS agencies can now allow their SaaS clients to cancel their subscriptions. **This feature is turned off by default because we believe taking cancellation requests and getting an opportunity to save the SaaS client is essential in churn-aversion.** But regardless, the decision rests with the agencies now! Agencies can enable this feature by going to their SaaS configurator. 

  
![](https://s3.amazonaws.com/cdn.freshdesk.com/data/helpdesk/attachments/production/48283853058/original/EXydpUSYh0jRtPZZbCAuKJDLeV7gfPi9XQ.png?1677443608)

  
Mark the checkbox to **Allow clients(sub-accounts) to cancel their subscriptions** and then hit the **Save Changes** button.

**Please Note:**

This will apply this setting to all SAAS accounts that will be created using your SAAS configurator moving forward.

  
This feature can also be controlled at a per-client level by Going to the **Agency Sidebar> Sub-Accounts> Scroll to the specific client> Click on their name or on Manage Client:**

[![](https://s3.amazonaws.com/cdn.freshdesk.com/data/helpdesk/attachments/production/48283853129/original/9AoVO1tjSy3tZiO9T9Pdp86r-psvGgEm1w.png?1677443737)](https://s3.amazonaws.com/cdn.freshdesk.com/data/helpdesk/attachments/production/48283851954/original/-B4BSvLsb6RMYvd1AhFHMdIAMamU3AE2sQ.png?1677441616)
  
  
![](https://s3.amazonaws.com/cdn.freshdesk.com/data/helpdesk/attachments/production/48283853190/original/M-C0JVaU2t_c5FRe7gKQpklWP0fPeVMpvw.png?1677443880)

  
Once you mark the checkbox to **Allow client (sub-account) to cancel their subscription,** They will be able to Cancel their Subscription. This setting will only apply to this sub-account and not all SAAS accounts created using your SAAS configurator moving forward. Sub-account, Once this checkbox is marked, your client will see a Modify Subscription button below their subscription details in **Settings> Company Billing:**

![](https://s3.amazonaws.com/cdn.freshdesk.com/data/helpdesk/attachments/production/48283853315/original/XhaDmc3F2wJFinQXHzHkr0lUWg6QYkcc3A.png?1677444056)

![](https://s3.amazonaws.com/cdn.freshdesk.com/data/helpdesk/attachments/production/48283853362/original/YJmN1TCM39ZEymD3Akcdm7YOMPCg3iRQrg.png?1677444178)  
Upon clicking **Cancel,** your client will see the following confirmation popup:  
![](https://s3.amazonaws.com/cdn.freshdesk.com/data/helpdesk/attachments/production/48283853420/original/opynSJ-8czUIdkHnfv9bGxrEInEgSnr9Mw.png?1677444302)

  
Once they click on **Confirm Cancellation,** They will see this message:  
![](https://s3.amazonaws.com/cdn.freshdesk.com/data/helpdesk/attachments/production/48283853447/original/rIoJvvzOmyRrCwitB3eV11oDYl1Au0pxAA.png?1677444384)

  
Whenever they try to access that canceled account they will see this message until they reactivate:  
  
![](https://s3.amazonaws.com/cdn.freshdesk.com/data/helpdesk/attachments/production/48283853919/original/HKf8Gd1WlX6sp90-psZrQeHnPyevgbAcuw.png?1677445552)

Your clients can reactivate their sub-accounts by clicking the reactivate button if they cancel their subscriptions. Also, they will have the option to change payment methods if required. 

  
Your client can also reach out to you using the agency's email under company settings if they ever get locked out erroneously. 

---

## **FAQ**

### **When my client cancels, will it automatically pause their sub-account?**

This behavior depends upon the following settings on the SaaS configurator: 

Therefore agencies can decide the behavior that suits them.

![](https://s3.amazonaws.com/cdn.freshdesk.com/data/helpdesk/attachments/production/48283853515/original/QQ9keW23Oy_rRKGHbuO_HpxhA9uwj1eguQ.png?1677444558)

### **What will happen on Stripe with the client subscription once they cancel?**

###  The subscription will also end on the Stripe side.

### **If my clients have remaining credits, what will occur?** 

Any remaining balance or credits in your client's account will be forfeited.

  