**Date Updated:** 2025-02-13T19:02:16.000Z

The Payment Received trigger is designed to act as a centralized mechanism for capturing all incoming payments across the CRM. It can be customized with filters to target specific use cases. This trigger helps businesses automate tasks, streamline processes, and efficiently respond to real-time customer transactions.

---

**TABLE OF CONTENTS**

* [What is the Payment Received Workflow Trigger?](#What-is-the-Payment-Received-Workflow-Trigger?)
* [Key Benefits Of Payment Received Workflow Trigger](#Key-Benefits-Of-Payment-Received-Workflow-Trigger)
* [How to use the Payment Received Trigger](#How-to-use-the-Payment-Received-Trigger)  
   * [Filters](#Filters)  
   * [If/Else Conditions](#If/Else-Conditions)  
   * [Custom Values](#Custom-Values)
* [Frequently Asked Questions](#Frequently-Asked-Questions)
* [Additional Benefits](#Additional-Benefits)

---

# **What is the Payment Received Workflow Trigger?**

  
The Payment Received trigger automates processes and actions based on incoming payments when used in a workflow. It can be configured to respond to all payment events across the CRM (ex: one-time purchases, subscription charges, invoices, etc), such as successful or failed transactions or particular products and payment sources.

  
The trigger starts a workflow instantly whenever a matching payment is received, allowing for automation of actions like sending confirmation emails, generating invoices, or updating customer records. Users can apply various filters to the trigger, such as transaction type, payment source, or product. This enables the creation of targeted workflows for specific scenarios, like subscription renewals, or failed payments.

  
By using if/else conditions in the Workflow, different actions can be executed in very specific situations depending on the payment characteristics, such as the amount, source, or transaction status. The workflow actions can also capture payment data for analysis and reporting purposes. By monitoring incoming payments and their attributes, businesses can gain insights into sales performance, customer behavior, and potential areas for improvement.

---

## **Key Benefits Of Payment Received Workflow Trigger**

  
The Payment Received trigger offers numerous usage cases and benefits, helping businesses automate processes, improve customer experience, and gain insights from payment data. Some common usage cases and their benefits include:

  
* **Automated payment confirmation:** Send customers automated confirmation emails or messages when Payment is processed, which enhances customer satisfaction.
* **Subscription management:** Automatically update subscription status in the system when a subscription payment is successful or failed, which increases business efficiency by streamlining subscription management.
* **Payment failure resolution:** Automatically notify customer support or sales teams to address and assist the Customer when a payment failure occurs; resolve payment issues quickly.

---

# **How to use the Payment Received Trigger**
  
  
**Step 1:** Inside a workflow, add a workflow trigger called **Payment Received.**

  
![](https://s3.amazonaws.com/cdn.freshdesk.com/data/helpdesk/attachments/production/155041535027/original/LuaYlXLD0wUPr6GAtd8O9TKuYMunxgXfEA.png?1739444985)
  
  
Click "add filter" to choose a filter. Then click "add filter" again to add the  Sub-filters. 

---

## **Filters**

  
You can make your Workflow trigger more specific using filters. Here is a table of all the available filters and sub-filters.

  
| Trigger                                       | Filter                             | Options at Filter Level | Sub-Filter Level 1                          | Options at Sub-Filter Level 1 | Operators  |
| --------------------------------------------- | ---------------------------------- | ----------------------- | ------------------------------------------- | ----------------------------- | ---------- |
| Payment Received                              | Payment Source                     | Invoice                 | Sub-Source                                  | Text2Pay link                 | is, is not |
| One-time invoice                              |                                    |                         |                                             |                               |            |
| Recurring template                            |                                    |                         |                                             |                               |            |
| Funnel/ Website                               | Sub-Source                         | One-step order form     |                                             |                               |            |
| Two-step order form                           |                                    |                         |                                             |                               |            |
| Upsell                                        |                                    |                         |                                             |                               |            |
| Transaction type                              | Customer present/first transaction |                         |                                             |                               |            |
| Customer not present/subscription transaction |                                    |                         |                                             |                               |            |
| Calendar                                      | Calendar                           | Calendar names          |                                             |                               |            |
| Global Product                                | Global product Names               | Price                   | Prices Names as per selected Global Product |                               |            |
| Payment status                                | Success                            | \---                    |                                             |                               |            |
| Failed                                        |                                    |                         |                                             |                               |            |

  
For example, if you want the workflow to trigger when a two-step order form is submitted, you select (1) Payment Source > (2) is > (3) Funnel and then you select add filter > (4) Sub-Source > (5) is > (6) two-step order form.

  
![](https://s3.amazonaws.com/cdn.freshdesk.com/data/helpdesk/attachments/production/155038871990/original/jIbyU9wy4QW1uUfU59g0Oe0Lj9gvorYF8g.png?1735067718)

---

## **If/Else Conditions**

  
Once you have added your desired set of Filters and Sub-Filters to your workflow trigger, you can add an If/Else Condition for Payment if you need to branch out the Workflow based on certain conditions. 

  
![](https://s3.amazonaws.com/cdn.freshdesk.com/data/helpdesk/attachments/production/155041545885/original/t7AzOXeC_h2Ny9inaeFgWD2IvemRTkKBPw.gif?1739451375)
  
  
This Table explains the possible If/Else Conditions and their branches.

  
| If/Else Option | Action                                                                                                                       | Operator    | Options              |
| -------------- | ---------------------------------------------------------------------------------------------------------------------------- | ----------- | -------------------- |
| Payment        | Product                                                                                                                      | is, is not  | Global product Names |
| Funnel/Website | Funnel/Website names                                                                                                         |             |                      |
| Calendar       | Calendar names                                                                                                               |             |                      |
| Source         | Invoice, Funnel, Website, Calendar                                                                                           |             |                      |
| Payment status | success/failed                                                                                                               |             |                      |
| Amount         | Equal to, is not equal to, Greater than, Greater than or equal to, Less than, Less than or equal to, is not empty, is empty. | Amount paid |                      |

---

## **Custom Values**

  
After adding and configuring the Payment Received Workflow trigger, the workflow actions have access to a set of Custom Values that you can populate within SMS, Emails, Internal Notifications, etc. This Table explains the custom values in detail.

  
| Custom Values Category             | Custom Values Name (Custom Value Group Name) | Custom Values within Group     | Value              |
| ---------------------------------- | -------------------------------------------- | ------------------------------ | ------------------ |
| **Payment**                        | Source                                       |                                | {{payment.source}} |
| Currency Symbol                    | {{payment.currency\_symbol}}                 |                                |                    |
| Currency Code                      | {{payment.currency\_code}}                   |                                |                    |
| **Customer (**Custom Values Group) | ID                                           | {{payment.customer.id}}        |                    |
| First Name                         | {{payment.customer.first\_name}}             |                                |                    |
| Last Name                          | {{payment.customer.last\_name}}              |                                |                    |
| Name                               | {{payment.customer.name}}                    |                                |                    |
| Email                              | {{payment.customer.email}}                   |                                |                    |
| Phone                              | {{payment.customer.phone}}                   |                                |                    |
| Full Address                       | {{payment.customer.address}}                 |                                |                    |
| City                               | {{payment.customer.city}}                    |                                |                    |
| State                              | {{payment.customer.state}}                   |                                |                    |
| Country                            | {{payment.customer.country}}                 |                                |                    |
| Postal Code                        | {{payment.customer.postal\_code}}            |                                |                    |
| **Invoice** (Custom Values Group)  | Name                                         | {{payment.invoice.name}}       |                    |
| Number                             | {{payment.invoice.number}}                   |                                |                    |
| Issue Date                         | {{payment.invoice.issue\_date}}              |                                |                    |
| Due Date                           | {{payment.invoice.due\_date}}                |                                |                    |
| URL                                | {{payment.invoice.url}}                      |                                |                    |
| Recorded By                        | {{payment.invoice.recorded\_by}}             |                                |                    |
| Sub-Total                          |                                              | {{payment.sub\_total\_amount}} |                    |
| Discount Amount                    | {{payment.discount\_amount}}                 |                                |                    |
| Coupon Code                        | {{payment.coupon\_code}}                     |                                |                    |
| Tax Amount                         | {{payment.tax\_amount}}                      |                                |                    |
| Created On                         | {{payment.created\_on}}                      |                                |                    |
| Total Amount                       | {{payment.total\_amount}}                    |                                |                    |
| Transaction ID                     | {{payment.transaction\_id}}                  |                                |                    |
| Status                             | {{payment.payment\_status}}                  |                                |                    |
| Gateway                            | {{payment.gateway}}                          |                                |                    |
| Card Last 4 Digits                 | {{payment.card.last4}}                       |                                |                    |
| Card Brand                         | {{payment.card.brand}}                       |                                |                    |
| Method                             | {{payment.method}}                           |                                |                    |

  
---

## **Frequently Asked Questions**

  
**What is the sub-source filter?**

  
When you select a source like funnels/websites/invoices, they can have sub-sources, like a payment from the funnel can be coming either via a one-step order form, a two-step order form, or an upsell. You can use these sub-source filters to define the Payment's origin.

  
**Will this trigger include the initial subscription payment and subsequent subscription payments as well?** 

  
Yes, the trigger will fire whenever a payment is received from the end customer directly on an order form submission and when the subscription is charged in the background.

  
**What does the Customer present/first transaction mean and the Customer not present/subscription transaction?**

  
We are categorizing the transaction type into two categories

* **Customer present /first transaction** \- This includes the transactions where the end customer is on-session and making the Payment. This consists of all one-time purchases and the first order placement for a subscription product.
* **Customer not present / subscription transaction** \- This includes the transaction types which run in the background after a subscription has already been created. For example, if a customer purchases a recurring product with a 14-day trial period. The transaction is done while purchasing the recurring product ($0 transaction in this case) would fall into the Customer present/first transaction. After 14 days, when the trial period is over, and you charge $100 for the recurring product, the $100 transaction would fall into the Customer not present/subscription transaction category.

  
**How can I configure the trigger for successful subsequent subscription transactions?**

  
Since the subscriptions can be created in a funnel or website, we can create a trigger for Payment Received and apply the following filters for achieving the use case. The source type is Funnel/Website. The transaction type is "Customer not present/subscription transaction." The payment status filter can filter successful or failed payments per the use case.

  
![](https://s3.amazonaws.com/cdn.freshdesk.com/data/helpdesk/attachments/production/155041546117/original/7l-LgbEmh0f0FKJXnSMQQaI9SLxv8aWYFw.png?1739451471)
  
  
**Will failed payments also be captured in this trigger?** 

  
Yes, by default, without any filters, the trigger runs upon successful and failed payment attempts. For specific use cases around success/failed payments only, we can apply the "Transaction status" filter and set it to either success/failed as per the use case.

  
![](https://s3.amazonaws.com/cdn.freshdesk.com/data/helpdesk/attachments/production/155041546210/original/xyXYNTCf_UL6-vTxallLYkcJpPrgJmeFpg.png?1739451511)
  
  
**I have configured the trigger and selected a specific product in the filters. Does this mean that the trigger will fire off when that product is sold anywhere?**

  
If you have configured the trigger and set the filter for a specific product, it will fire off only when that product is sold in funnels/website/invoices. Using the transaction status filter, we can define whether the trigger should work when the purchase is successful or the purchase is a failure.

---

## Additional Benefits

  
* **Dunning management:** Automatically trigger dunning email sequences for customers with failed subscription payments. Improves revenue recovery by addressing payment failures promptly, reduces churn, and enhances customer retention.
* **Customer segmentation:** Use payment data to create customer segments based on purchasing behavior, such as high-value customers or frequent buyers. Enables targeted marketing campaigns, helps identify upsell or cross-sell opportunities, and facilitates personalized customer experiences.
* **Sales performance tracking:** Monitor payment data to track sales performance and identify trends, such as best-selling products, seasonal fluctuations, or customer preferences. Provides valuable insights for strategic decision-making, helps optimize sales strategies, and drives revenue growth.
* **Integration with accounting systems:** Automatically update accounting records with payment information using outbound webhooks, such as invoicing, revenue recognition, or tax calculations. Ensures accurate financial reporting, streamlines accounting processes, and reduces manual data entry.
* **Handling trial period transactions:**The Payment Received trigger effectively manages transactions involving trial periods for subscription products, such as a 14-day trial. In this example, when a customer signs up for the trial and pays $0 upfront, the trigger categorizes this as a customer present transaction since they are on-session and entering their payment information. After the 14-day trial ends, the customer is charged $100 automatically without entering their payment details again. This subsequent transaction is considered a customer not present transaction, as it occurs in the background. The Payment Received trigger allows businesses to track and automate workflows around trial period transactions accurately. By efficiently handling trial period transactions, businesses can enhance customer experience, improve subscription management, and reduce manual intervention, increasing customer satisfaction and retention.
* **Integrating Text2Pay links:** The Payment Received trigger supports Text2Pay links as a payment source, enabling businesses to automate workflows for payments received through text message-based methods. By incorporating Text2Pay links in the trigger's configuration, businesses can effectively manage and respond to these transactions, improving the overall customer experience and streamlining payment processing. Utilizing Text2Pay links with the Payment Received trigger allows businesses to reach a wider audience, expedite payment processing, and simplify customer communication, ultimately leading to increased revenue and customer loyalty.