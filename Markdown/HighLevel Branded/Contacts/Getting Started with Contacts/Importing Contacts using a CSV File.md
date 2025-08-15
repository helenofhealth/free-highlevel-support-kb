**Date Updated:** 2025-04-24T17:34:49.000Z

This article shows you how to import contacts into HighLevel using a CSV file. You’ll learn how to upload, map, and confirm your data, and optionally choose to import Opportunities alongside Contacts.

  
**IMPORTANT**: In HighLevel, importing is supported only through the CSV (.csv) file format. Other file types like Excel or Google Sheets are not accepted. Please refer to this article to learn more about [](https://help.gohighlevel.com/support/solutions/articles/48000982206-csv-file-format-for-importing-contacts-and-opportunities)[CSV File Format for Importing Contacts and Opportunities](https://gohighlevelassist.freshdesk.com/support/solutions/articles/155000005143-csv-file-format-for-importing-contacts-and-opportunities)[](https://help.gohighlevel.com/support/solutions/articles/48000982206-csv-file-format-for-importing-contacts-and-opportunities)[](https://help.gohighlevel.com/support/solutions/articles/48000982206-csv-file-format-for-importing-contacts-and-opportunities)

---

**TABLE OF CONTENTS**

* [Prerequisites for Importing Contacts](#Prerequisites-for-Importing-Contacts)
* [Common Mistakes to Avoid](#Common-Mistakes-to-Avoid)
* [Importing Contacts](#Importing-Contacts)  
   * [Step 1: Navigate to the Contacts Tab](#Step-1%3A-Navigate-to-the-Contacts-Tab)  
   * [Step 2: Select What to Import](#Step-2%3A%C2%A0Select-What-to-Import)  
   * [Step 3: Upload Your CSV File](#Step-3%3A%C2%A0Upload-Your-CSV-File)  
   * [Step 4: Mapping Column to Fields](#Step-4%3A%C2%A0Mapping-Column-to-Fields)  
   * [Step 5: Verify, Confirm, and Finalize Selection](#Step-5%3A-Verify,-Confirm,-and-Finalize-Selection)
* [Optional: Import Contacts & Opportunities](#Optional%3A-Import-Contacts-&-Opportunities)
* [Monitor Import Status](#Monitor-Import-Status)
* [Frequently Asked Questions](#Frequently-Asked-Questions)
* [Related Articles](#Related-Articles)

---

## **Prerequisites for Importing Contacts**

  
Before starting the import process, make sure you meet the following requirements:  
  
* **User Permissions:** Only users with **Admin** access can import contacts.
* **File Format:** The file must be in **CSV (.csv) format**.
* **File Size Limit:** The CSV file should be **under 30 MB**. If it's larger, split it into smaller files.
* **Single Sheet Requirement:** Your CSV file must contain **only one sheet/tab**.
* **CSV Requirement**: The first row should **NOT** be blank! Include a header row in which at least one column header corresponds to a field in the system.

---

## **Common Mistakes to Avoid**

  
❌ **Mismatched headers**: Ensure CSV headers match system fields.

  
❌ **Blank required fields**: Every row should have at least one required field (Name, Email, or Phone).

  
❌ **Using special characters in phone numbers**: Remove spaces, dashes, or letters.

  
❌ **Duplicate records within CSV**: Clean the list before importing.

---

## **Importing Contacts using CSV File Format**

  
Importing contacts into HighLevel is the fastest way to bring your leads, clients, or customer lists into the platform. Whether you're switching from another CRM, onboarding new clients, or setting up your first marketing campaign, the import tool lets you upload and organize contacts quickly using a simple CSV file. You can also choose to import opportunities simultaneously, making your pipeline setup even smoother.
  
  
### **Step 1:** Navigate to the Contacts Tab

  
From the navigation toolbox, click on the **Import Contacts** button.

  
![](https://s3.amazonaws.com/cdn.freshdesk.com/data/helpdesk/attachments/production/155045268769/original/qntGJzsHbNyAo4uqr_KzH2KJyDyMv6lnkg.png?1744890922)
  
  
### **Step 2:** Select What to Import

  
Choose whether you’re importing only **Contacts** or both Contacts and Opportunities.

  
![](https://s3.amazonaws.com/cdn.freshdesk.com/data/helpdesk/attachments/production/155045269232/original/hblK0LKqfhz9WHiZfO5xoO0UMuxaLhHALg.png?1744891201)
  
  
### **Step 3:** Upload Your CSV File

  
**After selecting to import Contacts, click Next, then upload your CSV file and select the correct import type depending on whether you’re adding new contacts or updating existing ones.**

  
![](https://s3.amazonaws.com/cdn.freshdesk.com/data/helpdesk/attachments/production/155045270049/original/vQyHg0jDGj9TG88kbdLBy_IItrA-4ZWVFQ.gif?1744891799)
  
  
**Note**: When updating contacts, HighLevel checks for existing records based on the following order:  
Contact ID → Email → Phone.  
This matching order ensures accurate updates and avoids duplicates.  
You can change your deduplication settings or learn more about [Allow Duplicate Contacts (Contact Deduplication Preferences)](https://help.gohighlevel.com/support/solutions/articles/48001181714-allow-duplicate-contact-explained)
  
  
### **Step 4:** Mapping Column to Fields

  
Ensure each column in your file is correctly mapped to the corresponding field in the system. A few things to note:

1. Checking the "Don't update Empty Values" checkbox will not update any field if the imported file has empty values and the field does have some value for the opportunity.
2. If you decide not to import a certain field, you can choose to keep it unmapped and check the box on the bottom to proceed. -"Please ensure all mandatory fields are mapped. To proceed, either map all fields or choose Don't import data for unmapped columns."
3. If Contacts and Opportunities are on the same line in the CSV, they will be automatically mapped to each other.

  
![](https://s3.amazonaws.com/cdn.freshdesk.com/data/helpdesk/attachments/production/155045270487/original/0Kj5Ar-TSLDpndJhF8UKibEgkC1QbQZF8g.gif?1744892075)
  
  
### **Step 5**: Verify, Confirm, and Finalize Selection

  
Finalize the setup by reviewing your preferences, checking field mappings, and confirming consent before starting the import. This final step ensures that contacts are correctly tagged, sorted, and added to workflows, with your data fully verified.

  
**Preferences**: Optional Actions Before Import

  
* Create a SmartList for new contacts
* Add imported contacts to a workflow
* Tag imported contacts for easy segmentation

  
Review your Field Mapping. Make sure all **mandatory fields** are correctly mapped. Confirm that **custom fields** are assigned as intended. Optional: Unmapped columns will be ignored automatically.

  
![](https://s3.amazonaws.com/cdn.freshdesk.com/data/helpdesk/attachments/production/155045271590/original/VMvcfndMIiLbhM1kZ1_xbnDXXUo-xeLpXQ.gif?1744892718)

---

## **Optional: Import Contacts & Opportunities**

  
If your CSV includes both contact and deal (opportunity) information, you can import both at once using the same flow. This is especially useful if you're onboarding new leads directly into your sales pipeline and want to associate them with a stage or deal value during the import. The process remains exactly the same as importing contacts, the only difference is selecting both "Contacts" and "Opportunities" during the initial import setup.

  
After clicking the **Import** button on the Contacts page, you’ll be prompted to select objects to import. Simply check both and proceed with the same steps as stated above. 

  
![](https://s3.amazonaws.com/cdn.freshdesk.com/data/helpdesk/attachments/production/155045272006/original/svNfsDr0fNSalxqv41yASWcbrzcoJg_Aww.png?1744893094)
  
  
**Tip**: Your CSV must include Opportunity-related columns (e.g., Pipeline, Stage, Status, Opportunity Name) for that data to be created correctly. You can leave fields unmapped if not needed.

---

## **Monitor Import Status**

  
* You can monitor the progress and status of the import via the Contacts and Opportunities **Bulk Actions** Pages.
* Both contacts and opportunities imports will appear in the same place under **Bulk Actions.**
* Click on the "**Show Stats**" button to view the Stats of the import - you can also download the error log and view further details about the error and how to fix them in the "**Error**" tab.

  
![](https://s3.amazonaws.com/cdn.freshdesk.com/data/helpdesk/attachments/production/155045272144/original/FDJfjgAB0C83p5q7Cc62HjX-HkxheDGMrg.png?1744893191)

---

## **Frequently Asked Questions**

  
**Q: Can I import without email or phone?**  
You need at least one of these: name, email, or phone to create a contact.

  
**Q: Can I skip some CSV columns?**  
Yes, just leave them unmapped during field matching.

  
**Q: Can I update contact records?**  
Yes, choose “Update” or “Create and Update” and match based on contact ID or email.

  
**Q: Where do I find previous imports?**  
Go to **Bulk Actions** to view your import history.

---

## **Related Articles**

* [Importing Opportunities using a CSV file](https://gohighlevelassist.freshdesk.com/support/solutions/articles/155000002517-importing-opportunities-using-a-csv-file)
* [Allow Duplicate Contacts (Contact Deduplication Preferences)](https://help.gohighlevel.com/support/solutions/articles/48001181714-allow-duplicate-contact-explained)
* [CSV File Format for Importing Contacts and Opportunities](https://gohighlevelassist.freshdesk.com/support/solutions/articles/155000005143-csv-file-format-for-importing-contacts-and-opportunities)