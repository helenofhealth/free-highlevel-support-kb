**Date Updated:** 2025-04-09T02:14:19.000Z

This article explains the **"Create Contact"** workflow action, a powerful tool that automates the creation and updating of contact records in your CRM. You will learn what this action does, its key benefits, how to configure it step-by-step, and real-world use cases. Finally, we address common questions to help you maximize its potential.

---

**TABLE OF CONTENTS**

* [What is Create Contact Workflow Action](#What-is-Create-Contact-Workflow-Action)
* [Key Benefits of Create Contact Workflow Action](#Key-Benefits-of-Create-Contact-Workflow-Action)
* [Configuring the Create Contact Workflow Action](#Configuring-the-Create-Contact-Workflow-Action)  
   * [Name Your Action](#Name-Your-Action)  
   * [Select Fields](#Select-Fields)  
   * [Standard Fields](#Standard-Fields)  
   * [Custom Fields](#Custom-Fields)
* [Use Cases](#Use-Cases)[](#Frequently-Asked-Questions)
* [Frequently Asked Questions](#Frequently-Asked-Questions)

---

# **What is Create Contact Workflow Action**

  
The Create Contact workflow action enables businesses to automatically create new contact records or update existing ones based on predefined criteria. By capturing and maintaining accurate contact information, this action ensures seamless communication and data management. It is a cornerstone for automating workflows that involve customer onboarding, lead management, and other contact-based activities.

---

## **Key Benefits of Create Contact Workflow Action**

  
* **Improved Data Accuracy:** Ensures that contact records are always up-to-date, reducing errors and duplications.
* **Streamlined Processes:** Automates the manual task of adding or updating contact details, saving time and effort.
* **Enhanced Communication:** Enables timely follow-ups and personalized communications by maintaining accurate contact information.
* **Customizable Fields:** Supports standard and custom fields, allowing businesses to tailor contact records to their specific needs.
* **Seamless Integration:** Easily integrates with other workflow actions and triggers, creating robust automation processes.

---

## **Configuring the Create Contact Workflow Action**

  
### **Access Workflow Settings**

  
Navigate to the workflow builder inside automation section of your CRM. Create a new workflow from scratch or select the existing workflow where you want to implement the **"Create Contact"** workflow action.
  
  
### **Add a New Action**

  
Click **“+”** icon and select Create Contact from the dropdown menu.  
  
![](https://s3.amazonaws.com/cdn.freshdesk.com/data/helpdesk/attachments/production/155039310054/original/WuFv53oy7nz43NidBrihXSA-VHDWn73uZw.png?1736153467)

  
### **Name Your Action**

  
Provide a descriptive name, such as “Create Contact from Web Form.”  
  
![](https://s3.amazonaws.com/cdn.freshdesk.com/data/helpdesk/attachments/production/155039310124/original/yIUzSZ0til10P3zvfOfYySrAuYAzA94NFg.png?1736153517)

  
### **Select Fields**

  
Configure the fields to include in the contact creation or update process:

  
### **Standard Fields**

  
Examples include First Name, Last Name, Email, Phone, and Address.  
  
![](https://s3.amazonaws.com/cdn.freshdesk.com/data/helpdesk/attachments/production/155039310202/original/nrd2uo6Bpw7q9JOC2PzN9yzKPz1tHP98XA.png?1736153562)

  
### **Custom Fields**

  
Add unique fields specific to your organization, such as “Membership ID” or “Referral Source.”  
  
![](https://s3.amazonaws.com/cdn.freshdesk.com/data/helpdesk/attachments/production/155039310264/original/ZgS3qv1q1xL2KKE9rKybCq_mOEmKpUYYog.png?1736153616)

---

### **Save the Configuration**

  
Click the **"Save"** button to confirm your setup.

  
### **Test and Publish**

  
Validate the workflow with test data to ensure it functions as expected. Once verified, enable the Publish toggle to activate the workflow.

---

## **Use Cases**

  
### **Automating Contact Creation from Web Forms**

  
**Scenario:** A business wants to capture customer information from web form submissions and create or update contact records automatically.

  
**Action Setup:**

  
* **Action:** Create Contact.
* **Fields:** First Name, Last Name, Email, Phone, City, Country.

  
**Outcome:** The workflow creates or updates contact records in the CRM and notifies the sales team for follow-ups.

  
![](https://s3.amazonaws.com/cdn.freshdesk.com/data/helpdesk/attachments/production/155039343561/original/TIFnSKhBhNfXN0OC5QIiycpiPtHLKFWzNQ.png?1736175733)

  
---

### **Updating Contact Records After Purchases**

  
**Scenario:** When a customer makes a purchase, their CRM profile needs to be updated with transaction details.

  
**Action Setup:**

  
* **Action:** Create Contact.
* **Fields:** Full Name, Email, Purchase History (Custom Field).

  
**Outcome:** The workflow updates the customer’s profile with their latest purchase and tags them as “Active Customer.”

---

### **Lead Management from External Data Sources**

  
**Scenario:** Leads from a third-party platform are imported into the CRM, and their records need to be created or updated automatically.

  
**Action Setup:**

  
* **Action:** Create Contact.
* **Fields:** Business Name, Contact Source, Phone, Email.

  
**Outcome:** The workflow ensures that all leads are accurately recorded in the CRM with relevant details, ready for follow-up.

---

### **Onboarding New Customers**

  
**Scenario:** A subscription-based business wants to create a contact record for each new customer and assign them to an onboarding specialist.

  
**Action Setup:**

  
* **Action:** Create Contact.
* **Fields:** First Name, Last Name, Subscription Tier (Custom Field), Email.

  
**Outcome:** The workflow creates the contact record, assigns it to the onboarding team, and sends a welcome email.

---

### **Capturing Event Registrations**

  
**Scenario:** Attendee information from event registration forms needs to be recorded in the CRM for tracking and communication.

  
**Action Setup:**

  
* **Action:** Create Contact.
* **Fields:** Full Name, Email, Event Name (Custom Field).

  
**Outcome:** The workflow creates contact records for all attendees and tags them with the event name for future engagement.

---

## **Frequently Asked Questions**

  
**Q. What happens if the contact already exists?**

The Create Contact action updates the existing record with new information, ensuring data consistency and avoiding duplicates.
  
  
**Q. Can I use this action with custom fields?**

Yes, the action supports both standard and custom fields, allowing you to tailor contact records to your specific requirements.
  
  
**Q. How can I prevent duplicate records?**

The action uses matching criteria, such as email or phone number, to identify existing contacts and update their records instead of creating new ones.
  
  
**Q. Can this action be combined with other workflow actions?**

Absolutely. The Create Contact action integrates seamlessly with actions like **“Send Email”** or **“Assign Task”** to build comprehensive workflows.
  
  
**Q. Is it possible to notify teams when a contact is created or updated?**

Yes, you can add a notification action within the same workflow to inform relevant teams about the new or updated contact.
  
  