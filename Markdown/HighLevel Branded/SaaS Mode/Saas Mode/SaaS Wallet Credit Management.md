**Date Updated:** 2025-06-14T01:27:26.000Z

####   

####   

#### **Covered in this article:**

#### [**What is SaaS Wallet?**](#What-is-SaaS-Wallet?)

#### **[Where can the wallet be accessed from?](#Where-can-the-wallet-be-accessed-from?)**

#### **[How to view the wallet transaction history?](#How-to-view-the-wallet-transaction-history?)**

#### [**How to Recharge Wallet?**](#How-to-Recharge-Wallet?)

#### [1\. Auto Recharge Settings](#1.-Auto-Recharge-Settings)

#### [2\. Charge Client's Card Manually (Add Balance)](#2.-Charge-Client's-Card-Manually-%28Add-Balance%29)

#### [3\. Monthly Complimentary Credits](#3.-Monthly-Complimentary-Credits)

#### [4\. Add Complimentary Credits from Agency View](#4.-Add-Complimentary-Credits-from-Agency-View)

####   
[**How to Remove Credits from the wallet?**](#How-to-Remove-Credits-from-the-wallet?)

#### [1\. Complimentary Credits](#1.-Complimentary-Credits)

#### [2\. Non-Complimentary Credits](#2.-Non-Complimentary-Credits)[](#How-to-Issue-Refunds-for-Non-Complimentary-Credits)

####   

####   
[**How to Issue Refunds for Non-Complimentary Credits**](#How-to-Issue-Refunds-for-Non-Complimentary-Credits)

####   
[**Wallet Recharge Retries**](#Wallet-Recharge-Retries)

#### [1\. SaaS Wallets (for telephone & email rebilling)](#1.%C2%A0SaaS-Wallets-%28for-telephone-&-email-rebilling%29)

#### [2\. Agency Wallets (for ISV)](#2.%C2%A0Agency-Wallets-%28for-ISV%29)

  
---

# **What is SaaS Wallet?**

  
To charge the client for Twilio and Email rebilling, the system uses their wallet. The agency owner/ client recharges their wallet using the client's credit card which adds messaging credits to the location wallet. Each time a message/ email is sent, call is made, or a phone number is purchased, the wallet credits are debited.

  
**Please note:** 

Some charges in the wallet may appear after **6 - 24 hours**.

  
The wallet is recharged when it reaches the minimum balance set in the Company Billing settings. The client's card is attached to the wallet for all charges. The wallet can also be recharged with complimentary (free) monthly/ one-time credits.

  
Now, each time a message is sent, Twilio / Mailgun will charge the agency, and the system will charge the client's wallet based on rebilling settings. So for example the client sent 100 messages worth $10 and rebilling was set to 5x, the agency will be charged $10 by Twilio, and the client's wallet will be charged $50.

  
**Please note:** 

When the wallet is recharged, the client's card is charged and these charges are sent into the Agency's Stripe account. So the client is paying the agency for these wallet credits.
  
  
---

# **Where can the wallet be accessed from?**

  
The wallet is found in the Subaccount Settings > Company Billing

  
![](https://s3.amazonaws.com/cdn.freshdesk.com/data/helpdesk/attachments/production/48179220627/original/r-cGcDfoBT7XnC_abUKNm_Ow2VnD_kVv6A.png?1642188595)
  
  
---

# **How to view the wallet transaction history?**

  
You can view the wallet transaction history from Settings > Company Billing > Credits > See Details:

  
![](https://s3.amazonaws.com/cdn.freshdesk.com/data/helpdesk/attachments/production/48179221231/original/TXqt8wBkRBOchmACU_YMdAKrYG2f-B_pfA.png?1642188770)
  
  
---

# **How to Recharge Wallet?**

  
The wallet can be recharged in several ways.

  
## **1\. Auto Recharge Settings**

  
In the Company Billing > Credits section, you can find the auto recharge settings with 2 options. The amount entered in the 'Auto Recharge with' field will be added to the wallet each time the balance is lower than the amount set in the 'when balance lower than' field.

  
![](https://s3.amazonaws.com/cdn.freshdesk.com/data/helpdesk/attachments/production/48179222076/original/LB4LFuJAKL9AnoirgKBlbEBMeNce505fQA.png?1642189100)
  
  
## **2\. Charge Client's Card Manually (Add Balance)**

  
Using the 'Add Balance' button in Company Billing, you can recharge the client's wallet. This method will charge the client's primary card added in the Company Billing settings

  
![](https://s3.amazonaws.com/cdn.freshdesk.com/data/helpdesk/attachments/production/48179223494/original/PsQIq28kR5TZ_O13q4a634VUEcjUhPQJhg.png?1642189572)
  
  
## **3\. Monthly Complimentary Credits**

  
If the subaccount is on a SaaS Plan, you can set an amount of credits to be granted to the subaccount on monthly basis. These credits will be added to the client's wallet each month. These credits can be modified for each SaaS Plan from the SaaS Configurator:

  
![](https://s3.amazonaws.com/cdn.freshdesk.com/data/helpdesk/attachments/production/48179224350/original/WiV2HJcC_3jecI3DCoeQGb3DyuocqdGEog.png?1642189881)
  
  
The amount for these credits can also be changed for each subaccount (which is on a SaaS Plan) individually. The individual settings can be accessed from Agency View > Accounts > View Details:

  
![](https://s3.amazonaws.com/cdn.freshdesk.com/data/helpdesk/attachments/production/48179224816/original/0s24US3LCvhVYQt3E9XEctFypBiJu_OYag.png?1642190032)
  
  
## **4\. Add Complimentary Credits from Agency View**

  
In the Agency View > Accounts > View Details > Manage Credits, you can also add complimentary credits to the client's wallet directly. These credits are not charged to anyone. Once the client uses these credits to send out messages/ calls, then the agency owner is charged for those messages/ calls, but the client is not charged since these credits were given for free.

  
![](https://s3.amazonaws.com/cdn.freshdesk.com/data/helpdesk/attachments/production/48179225579/original/3Dc5PvZJROUW2mKJirq29F9YIpO-M57XIA.png?1642190302)
  
  
---

# **How to Remove Credits from the wallet?**
  
  
## **1\. Complimentary Credits**

  
These credits can be removed by using the 'Debit' option in the Agency View > Accounts > View Details > Manage Credits. The Debit option only removes the balance from the wallet, it does not refund the amount in Stripe, so if you want to remove original (non-complimentary) credits, you will need to follow an additional step mentioned in the next paragraph.  
  
![](https://s3.amazonaws.com/cdn.freshdesk.com/data/helpdesk/attachments/production/48179226525/original/_esPD3ycS5qkglxxcQPc2q681OVesOgh2A.png?1642190596)
  
  
## **2\. Non-Complimentary Credits**

  
To remove these credits:   
  
1\. Use the same 'Debit' option mentioned above.  
  
2\. You will **_also_** need to issue a refund for these credits from your Stripe account by following the steps mentioned below.
  
  
---

## **How to Issue Refunds for Non-Complimentary Credits**

  
**1.** Go to the Stripe account connected in your Agency Settings > Stripe

  
[**2.** Find the client's Stripe customer associated with their subaccount ](https://help.gohighlevel.com/support/solutions/articles/48001207110-how-to-upgrade-downgrade-saas-plan-for-a-location#Finding-the-Stripe-Customer%3A)

  
**3.** In the 'Payments' section for this customer, find the payment for the addition of credits and click the 'Refund payment' button against that payment

  
![](https://s3.amazonaws.com/cdn.freshdesk.com/data/helpdesk/attachments/production/48179228361/original/qJlF0g2BYgjbz12TNQikaXPZ7h3Za8ashg.png?1642191183)

  
That's it, you're all set! :)
  
  
---

# **Wallet Recharge Retries**
  
  
## **1\.** **SaaS Wallets (for telephone & email rebilling)**

  
We will try to automatically charge the wallet a maximum of **7 times (7 attempts x 1 attempt/day).**

If all 7 attempts fail we will stop automatic retries.

* We will notify the agency admins
* We will notify the location admins
  
  
## **2\.** **Agency Wallets (for ISV)**

  
We will try to automatically charge the wallet a maximum of **12 times (3 days x 4 attempts/day).**

If all 12 attempts fail we will stop automatic retries

  
* We will notify the agency admins
  
  
**Please Note:** 

We are making this change because repeated retries were causing the suspension of Stripe accounts. Once we give up manual retries, users will be able to recharge manually and that will reset our counter and automatic retries will start again.

  