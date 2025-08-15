**Date Updated:** 2025-01-13T13:28:10.000Z

This article provides a detailed explanation of the **"Order Form Submission"** workflow trigger, a powerful tool for automating actions whenever a customer submits an order form. You will learn what this trigger does, its key benefits, how to configure it step-by-step, and real-world use cases. Finally, we’ll answer some common questions to help you get the most out of this feature.

---

**TABLE OF CONTENTS**

* [What is Order Form Submission Workflow Trigger](#What-is-Order-Form-Submission-Workflow-Trigger)
* [Key Benefits of Order Form Submission Trigger](#Key-Benefits-of-Order-Form-Submission-Trigger)
* [Configuring the Order Form Submission Workflow Trigger](#Configuring-the-Order-Form-Submission-Workflow-Trigger)  
   * [Name Your Trigger](#Name-Your-Trigger)  
   * [Set Filters (Optional):](#Set-Filters-%28Optional%29%3A)  
         * [In Funnel/Website](#In-Funnel/Website)  
         * [Submission Type](#Submission-Type)
* [Use Cases](#Use-Cases)
* [Frequently Asked Questions](#Frequently-Asked-Questions)

  
---

# **What is Order Form Submission Workflow Trigger**

  
The Order Form Submission workflow trigger activates whenever a customer completes and submits an order form through a funnel or website. This trigger helps businesses automate essential tasks like sending order confirmations, updating CRM records, notifying team members, and even triggering post-purchase upsells. By automating these processes, businesses can improve efficiency, enhance the customer experience, and ensure timely follow-ups.

---

## **Key Benefits of Order Form Submission Trigger**

  
Check out why this trigger is a game changer :  
  
* **Automated Order Management:** Streamlines order processing by automating tasks such as confirmation emails, record updates, and internal notifications.
* **Improved Customer Experience:** Ensures customers receive immediate confirmation and relevant follow-ups, enhancing trust and satisfaction.
* **Flexible Configuration:** Allows businesses to customize workflows using filters like funnel, page, product, and submission type for precise automation.
* **Increased Sales Opportunities:** Facilitates upsell and cross-sell campaigns by triggering follow-up actions based on the products purchased.
* **Accurate Data Capture:** Automatically updates CRM records, ensuring that customer information is always up-to-date and accurate.

---

## **Configuring the Order Form Submission Workflow Trigger**

  
Follow these steps to set up the Order Form Submission trigger in your workflow :

  
### **Access Workflow Builder**

  
Go to the **"Automation"** section in your CRM platform. Create a workflow from scratch or select the existing workflow where you would like to set up the Order Form Submission trigger.
  
  
### **Add a New Trigger**

  
Click **“Add New Trigger”** and select **"Order Form Submission"** from the list.

  
![](https://s3.amazonaws.com/cdn.freshdesk.com/data/helpdesk/attachments/production/155039635087/original/FGH3gbcRkgEf_9jcST7ZPZSusyC6G0m1bg.png?1736519992)

  
### **Name Your Trigger**

  
Enter a clear, descriptive name, such as “Order Form Submitted for John's Live Workshop"

  
![](https://s3.amazonaws.com/cdn.freshdesk.com/data/helpdesk/attachments/production/155039635120/original/gYUbpEM67ibi2DDKdBLI_NkLEBiCLGKUuw.png?1736520013)

  
### **Set Filters (Optional):**

  
Use filters to refine the conditions under which the workflow will activate:

  
![](https://s3.amazonaws.com/cdn.freshdesk.com/data/helpdesk/attachments/production/155039635219/original/i4tuzQ031voiLj3vbQJSx39In70V915Nrg.png?1736520049)

  
####   
**In Funnel/Website**

  
Select the specific funnel or website where the order form is located. You can also add an additional filter to select the specific page and also the specific product where you want to apply this trigger.  
  
![](https://s3.amazonaws.com/cdn.freshdesk.com/data/helpdesk/attachments/production/155039701838/original/UK9M7vZu_X3UeefEuNkDrElqorNRcR-tew.png?1736751534)  
**Page Is**

  
Choose a specific page in the funnel or website where the order form is hosted.

  
![](https://s3.amazonaws.com/cdn.freshdesk.com/data/helpdesk/attachments/production/155039701849/original/q9BYYs4LCZgpMtkiKhZVyZIT9PNo6VG9cw.png?1736751563)  
  
**Product Is**

  
Specify the product(s) linked to the order form to trigger the workflow only for those products.

  
![](https://s3.amazonaws.com/cdn.freshdesk.com/data/helpdesk/attachments/production/155039701872/original/MY8ie7S8NOwxyoDrkouedSs39uJfJvI8GA.png?1736751601)

  
---

#### **Submission Type**

  
The Submission Type filter is designed to activate the workflow trigger based on the specific type of order form submission a customer completes. This allows businesses to create highly tailored automations depending on how far a customer goes in the purchase process or what type of additional offer they accept during checkout.

  
Here’s a detailed explanation of the different submission types:

  
* **Bump**  
    
**What it means:** Triggered when a customer purchases a bump offer, which is an add-on product shown during the initial checkout process.  
    
**Why it’s useful:** Great for tracking and automating workflows around add-on products, such as sending personalized follow-up messages or cross-selling related products.
* **Opt-In**  
    
**What it means** **:** This type is triggered when a customer fills out their contact information (like name and email) but doesn’t complete the order.  
    
**Why it’s useful** **:** Ideal for abandoned cart workflows, this helps businesses follow up with potential customers who showed interest but didn’t finish their purchase, encouraging them to come back and complete the order.
* **Sale**  
    
**What it means** **:** This is triggered when a customer successfully completes a purchase by making a payment.  
    
**Why it’s useful** **:** Perfect for automating order confirmations, sending thank you emails, and initiating post-purchase follow-ups, such as upsell or feedback requests.
* **Upsell**  
    
**What it means** **:** Triggered when a customer accepts an upsell offer presented after the initial purchase.  
    
**Why it’s useful** **:** Helps businesses track and manage upsell campaigns, send upsell-specific order details, or notify internal teams about high-value customers who made additional purchases.

  
![](https://s3.amazonaws.com/cdn.freshdesk.com/data/helpdesk/attachments/production/155039701903/original/0tv0TE6AhermbCx-t5jo5E3r3FPVdVO6nQ.png?1736751638)

---

### **Finalizing and Activating the Workflow**

  
Once the filters are configured, click the **"Save"** button to finalize the trigger setup. Set the funnel to test mode and use dummy details to simulate an order submission, ensuring everything in the workflow works as expected. After successful testing, enable the **"Publish"** toggle to activate the workflow.

---

## **Use Cases**

  
Lets look at some examples where you can use this trigger:

  
### **Use Case #1 Order Confirmation and CRM Update**

  
**Scenario:** A business wants to automatically send an order confirmation email and update the customer’s CRM record upon purchase.

  
**Outcome:** The workflow sends a confirmation email to the customer, updates their CRM record with order details, and tags them for future marketing campaigns.

---

### **Use Case #2 Abandoned Cart Recovery**

  
**Scenario:** A business wants to follow up with customers who filled out their contact information but didn’t complete the order.

  
**Outcome:** The workflow sends a reminder email to the customer, offering an incentive (like a discount) to complete the purchase.

---

### **Use Case #3 Post-Purchase Upsell Campaign**

  
**Scenario:** A business wants to offer an upsell immediately after a purchase to maximize 

sales.

  
**Outcome:** The workflow sends an email offering an upsell product, with a limited-time discount to encourage immediate action.

---

### **Use Case #4 Internal Notification for High-Value Purchases**

  
**Scenario:** A sales team needs to be notified when a customer purchases a high-ticket 

product to ensure timely follow-up.

  
**Outcome:** The workflow sends an internal notification to the sales team, prompting them to reach out to the customer.

---

### **Use Case #5 Upsell and Bump Offer Tracking**

  
**Scenario:** A business wants to track the effectiveness of its upsells and bump offers during the checkout process.

  
**Outcome:** The workflow logs the upsell or bump offer acceptance in the CRM and sends a follow-up email to the customer.

---

## **Frequently Asked Questions**

  
**Q. Can I trigger multiple workflows for different submission types within the same funnel?**

Yes, you can set up separate workflows for each submission type (Optin, Sale, Upsell, Bump) by using specific filters to activate them accordingly.
  
  
**Q. How can I handle abandoned carts using this trigger?**

Use the **“Opt-in”** submission type filter to target customers who didn’t complete their purchase. You can then create a workflow that sends reminder emails or offers discounts to encourage them to complete the order.
  
  
**Q. Is it possible to track upsell conversions separately from main sales?**

Yes, by using the **“Upsell”** submission type filter, you can create a dedicated workflow to track and analyze upsell conversions.
  
  
**Q. How do I test the workflow before publishing it?**

You can set the funnel to test mode and use dummy card details to simulate an order form submission. This allows you to verify that the workflow is functioning correctly before making it live.
  
  
**Q. Can I send different confirmation emails based on the product purchased?**

Absolutely. You can use the **“Product Is”** filter to create separate workflows for different products and customize the confirmation emails accordingly.