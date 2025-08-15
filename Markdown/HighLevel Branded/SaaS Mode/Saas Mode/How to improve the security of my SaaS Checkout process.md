**Date Updated:** 2025-01-22T06:37:19.000Z

There are several steps you can take to enhance the security of your SaaS checkout. These measures can help prevent phishing scammers from signing up and misusing your SaaS sub-account.

  
**TABLE OF CONTENTS**

* [Step 1 - Use Funnel/Website v2](#Step-1---Use-Funnel/Website-v2)
* [Step 2 - Add Custom Authorization to your trial](#Step-2---Add-Custom-Authorization-to-your-trial)
* [Step 3 - Use LC Phone & LC Email](#Step-3---Use-LC-Phone-&-LC-Email)
* [Step 4 - Enable Phone Number & Email Verification by default](#Step-4---Enable-Phone-Number-&-Email-Validation-by-default)
* [Step 5 - Use Stripe Radar](#Step-5---Use-Stripe-Radar)  
   * [Useful rules we recommend](#Useful-rules-we-recommend)  
         * [3D Secure Authentication Rules](#3D-Secure-Authentication-Rules)  
         * [Block Rules](#Block-Rules)  
         * [Review Rules](#Review-Rules)
* [FAQ:](#FAQ%3A)  
   * [Q: I followed these steps but a scammer was still able to signup. What do I do?](#Q%3A-I-followed-these-steps-but-a-scammer-was-still-able-to-signup.-What-do-I-do?)  
   * [Q: What is Funnel/Website v2 and how does it enhance security?](#Q%3A-What-is-Funnel/Website-v2-and-how-does-it-enhance-security?)  
   * [Q: What is Custom Authorization and how does it work?](#Q%3A-What-is-Custom-Authorization-and-how-does-it-work?)  
   * [Q: Why should I consider using LC Phone & LC Email over Twilio or Mailgun?](#Q%3A-Why-should-I-consider-using-LC-Phone-&-LC-Email-over-Twilio-or-Mailgun?)  
   * [Q: How can I enable Phone Number & Email Verification for my SaaS signups?](#Q%3A-How-can-I-enable-Phone-Number-&-Email-Verification-for-my-SaaS-signups?)  
   * [Q: What is Stripe Radar and how does it help in fraud prevention?](#Q%3A-What-is-Stripe-Radar-and-how-does-it-help-in-fraud-prevention?)  
   * [Q: How can I set up rules in Stripe Radar for handling transactions?](#Q%3A-How-can-I-set-up-rules-in-Stripe-Radar-for-handling-transactions?)  
   * [Q: What action should I take if a flagged payment appears in Stripe Radar?](#Q%3A-What-action-should-I-take-if-a-flagged-payment-appears-in-Stripe-Radar?)

  
# Step 1 - Use Funnel/Website v2

If you're currently using HighLevel funnels & websites for SaaS sales, it's advisable to switch to v2 funnels & websites. The newer version supports native Stripe integration and 3D secure technology, ensuring a more secure checkout experience.

  
![](https://s3.amazonaws.com/cdn.freshdesk.com/data/helpdesk/attachments/production/155009989986/original/_3ABLUhxhsHSRmn_uyvJh3NgctFb4XF_QQ.png?1697131516)

  
# Step 2 - Add Custom Authorization to your trial

Adding an authorization amount to your SaaS products with a trial is the best way to ensure only real credit cards with enough balance are able to get through your signup process. 

  
You can enter an authorization amount on your sales funnel by going to funnel -> Products -> Additional Options -> Custom Authorization.

  
![](https://s3.amazonaws.com/cdn.freshdesk.com/data/helpdesk/attachments/production/155009990802/original/uVeQroA0MV1fGH7NAp6iH5__P7uEehqo-g.png?1697132231)

  
![](https://s3.amazonaws.com/cdn.freshdesk.com/data/helpdesk/attachments/production/155009990853/original/4nBOm8fAGyQ34wEgXSws_RD6TYHjsIzESw.png?1697132271)

  
A Custom Authorization is especially helpful when your SaaS product has a trial. It sim ply creates a payment intent and validates that the card is real and has sufficient balance. The customer is NOT charged and the payment is refunded immediately. 

  
Note
- Custom Authorization does NOT charge the customer. It creates a payment intent and immediately refunds it
- It's recommended to set the authorization amount equal to the monthly fee of your most basic plan.
  
  
# Step 3 - Use LC Phone & LC Email

  
Using Twilio or Mailgun is risky for SaaS agencies because of latency in rebilling. This allows scam artists and bad actors to rack up your Twilio & Mailgun usage before the location credits are debited. This latency is caused by delays in usage records and webhooks that we receive from Twilio or Mailgun. 

  
Using LC Phone & LC Email allows us to prevent that latency and also gives you access to additional security features like

1. Ramped usage for SMS, Email, VM drops, etc.
2. Maximum sending limits on Sub-accounts
3. Error rate, unsubscribe rate & complaint rate monitoring

  
[LC Email Ramp ](https://help.gohighlevel.com/support/solutions/articles/48001220605-what-is-lc-email-i-want-to-know-more#Ramp-Up-Model%3A)

[LC Phone Ramp ](https://help.gohighlevel.com/support/solutions/articles/48001213941-lc-phone-messaging-policy#1.-Ramp-Up-Model%3A)

[LC Email error thresholds & sending limit ](https://help.gohighlevel.com/support/solutions/articles/48001220605-what-is-lc-email-i-want-to-know-more#extend-sending-limit)

[LC Phone error thresholds ](https://help.gohighlevel.com/support/solutions/articles/48001213941-lc-phone-messaging-policy#2.-Spam-Message-handling%3A)

[LC Email Verification ](https://help.gohighlevel.com/en/support/solutions/articles/48001235221)

  
All these technologies run in the background to minimize the chances of bad actors misusing your SaaS sub-account.

  
Migration to LC Phone & LC Email is easier than you may think. 

  
[How do I migrate my agency and sub-account over to LC Phone?](https://help.gohighlevel.com/en/support/solutions/articles/48001204027)

[How to Migrate My Agency Over to LC - Email](https://help.gohighlevel.com/en/support/solutions/articles/48001222501)

  
# Step 4 - Enable Phone Number & Email Verification by default

  
Boost the security of future SaaS signups by enabling Phone Number and Email Verification. 

  
* Email Verification is mandatory by default for all SaaS signups.
* You can enable Phone Number verification for future SaaS signups by heading over to Agency Level -> Left Menu -> SaaS Configurator -> Security Settings -> Toggle : Verify Phone Number using a security code during sign-up
* To enable email verification for all your existing sub-accounts please head over to Agency Level -> Left Menu -> Settings -> Email Services -> Sub-Account Settings -> Enable Email Verification for all sub-accounts

  
# Step 5 - Use Stripe Radar

Stripe Radar is a fraud prevention suite integrated into the Stripe payment platform, utilizing machine learning algorithms trained on vast global data to detect and deter fraudulent transactions. It enables businesses to set custom rules to handle transactions based on specific parameters and provides detailed insights into flagged activities. Additionally, Radar offers features like adaptive acceptance, which dynamically requests added authentication for riskier payments, and a review dashboard for manual assessment. Integrated natively with Stripe, it offers a streamlined approach to online transaction security, reducing the need for third-party tools.

  
Stripe Radar is a paid product by Stripe but highly recommended for SaaS Agencies
  
  
[Stripe Radar](https://stripe.com/en-ca/radar)

  
Please log into your Stripe account and head over to Dasboard -> More -> Radar for Fraud Teams

  
![](https://s3.amazonaws.com/cdn.freshdesk.com/data/helpdesk/attachments/production/155009992667/original/ybHmh8pg5Q_5Tble9_IzDd5idyaHqPzFig.png?1697134292)

  
## Useful rules we recommend

You can add Radar rules by heading over to the rules tab

  
### **3D Secure Authentication Rules**

  
These rules will allow the payment to go through if 3D Secure is authenticated

  
![](https://s3.amazonaws.com/cdn.freshdesk.com/data/helpdesk/attachments/production/155009993558/original/c8R63SyPyTXmuKg5_-C5FW2Jh8O_Q5GU4Q.png?1697135590)
  
  
### **Block Rules**

  
These rules will block they payment altogether

  
![](https://s3.amazonaws.com/cdn.freshdesk.com/data/helpdesk/attachments/production/155009993599/original/IdCkpkdV5fOsCS9SX-bkKuIsigezFG8tcQ.png?1697135673)

  
### **Review Rules**

  
These rules will allow the payment to occur but they will be successful only if a human reviews and approves them

![](https://s3.amazonaws.com/cdn.freshdesk.com/data/helpdesk/attachments/production/155009993645/original/MNqV767sNLtdLYKxH3bHERszWOl4Lz1WcA.png?1697135770)

  
You can see all your pending reviews by heading over to the reviews tab in Radar. It looks like this

  
![](https://s3.amazonaws.com/cdn.freshdesk.com/data/helpdesk/attachments/production/155009993689/original/4kNj3tNRcl9hP5jwtqECh2cBCN0LgpkrMA.png?1697135899)

  
As an agency admin or owner you can approve or refund these payments manually. 

  
---

# **FAQ:**

  
## **Q: I followed these steps but a scammer was still able to signup. What do I do?**

  
A: All the rules mentioned above are best practices and they will prevent your SaaS sub-accounts from being misused in most cases. However, some bad actors might still be able to get through in rare instances. 

  
In such cases the best thing is to refund all fraudulent payments and specifically mark them as fraudulent. 

  
![](https://s3.amazonaws.com/cdn.freshdesk.com/data/helpdesk/attachments/production/155009994016/original/NuNsREtKzjWvqpGbTsTRt6xU7gIZC4hXrQ.png?1697136361)

  
![](https://s3.amazonaws.com/cdn.freshdesk.com/data/helpdesk/attachments/production/155009994056/original/1DGpk1rEatstJp4RhI8TWSsI--PmCXzYDQ.png?1697136456)

  
When refunding the payment please select it as "Fraudulent". This is VERY IMPORTANT. 

  
By refunding the payment and marking it as fraudulent Stripe Radar automatically gets smarter over time and prevents more scams from happening. 

  
It automatically 

* Adds the card fingerprint to your blocklist
* Adds the email ID to your blocklist
* Sends various signals like IP, email, card number, etc to Stripe which makes it more accurate over time

  
## **Q: What is Funnel/Website v2 and how does it enhance security?**

A: Funnel/Website v2 is an upgraded version of HighLevel funnels & websites. It supports native Stripe integration and 3D secure technology, which significantly improves the security of your SaaS checkout.
  
  
## **Q: What is Custom Authorization and how does it work?**

A: Custom Authorization is a feature that allows you to add an authorization amount to your SaaS products with a trial. It ensures that only real credit cards with sufficient balance can sign up. The customer is not charged; instead, a payment intent is created to validate the card's authenticity and immediately refunded.

## **Q: Why should I consider using LC Phone & LC Email over Twilio or Mailgun?**

  
A: Using Twilio or Mailgun can be risky due to latency in rebilling, which can be exploited by scammers. LC Phone & LC Email prevent this latency and offer additional security features like ramped usage, sending limits, and error rate monitoring.

  
## **Q: How can I enable Phone Number & Email Verification for my SaaS signups?**

A: You can enable these verifications through the Agency Level settings. For phone number verification, navigate to Settings -> Phone Integration. For email verification, go to Settings -> Email Services.

## **Q: What is Stripe Radar and how does it help in fraud prevention?**

A: Stripe Radar is a fraud prevention suite integrated into the Stripe payment platform. It uses machine learning algorithms to detect and deter fraudulent transactions. It allows businesses to set custom rules for transactions and provides insights into flagged activities.

  
## **Q: How can I set up rules in Stripe Radar for handling transactions?**

A: You can add Radar rules by heading over to the rules tab in your Stripe account. There are different types of rules, such as 3D Secure Authentication Rules, Block Rules, and Review Rules, to customize how transactions are handled.

## **Q: What action should I take if a flagged payment appears in Stripe Radar?**

A: If a payment is flagged in Stripe Radar, you can review it manually. As an agency admin or owner, you have the option to approve or refund these payments based on your assessment.

  