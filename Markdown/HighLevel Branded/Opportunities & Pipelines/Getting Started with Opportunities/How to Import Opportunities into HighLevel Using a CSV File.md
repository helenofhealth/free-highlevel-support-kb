**Date Updated:** 2025-04-24T17:37:00.000Z

This article will guide you through importing opportunities into HighLevel using a CSV file. Learn how to prepare your data, map fields, and ensure a smooth import process to keep your sales pipeline organized and up-to-date.

  
**IMPORTANT**: In HighLevel, importing is supported only through the CSV (.csv) file format. Other file types like Excel or Google Sheets are not accepted. Please refer to this article to learn more about [](https://help.gohighlevel.com/support/solutions/articles/48000982206-csv-file-format-for-importing-contacts-and-opportunities)[CSV File Format for Importing Contacts and Opportunities](https://gohighlevelassist.freshdesk.com/support/solutions/articles/155000005143-csv-file-format-for-importing-contacts-and-opportunities)[](https://help.gohighlevel.com/support/solutions/articles/48000982206-csv-file-format-for-importing-contacts-and-opportunities)[](https://help.gohighlevel.com/support/solutions/articles/48000982206-csv-file-format-for-importing-contacts-and-opportunities)[](https://help.gohighlevel.com/support/solutions/articles/48000982206-csv-file-format-for-importing-contacts-and-opportunities)

---

**TABLE OF CONTENTS**

* [Prerequisites for Importing Contacts](#Prerequisites-for-Importing-Contacts)
* [Common Mistakes to Avoid](#Common-Mistakes-to-Avoid)
* [Importing Opportunities via CSV ](#Importing-Opportunities-via-CSV%C2%A0)
* [How to Import Opportunities](#How-to-Import-Opportunities)  
   * [Step 1: Navigate to the Opportunities Tab](#Step-1%3A%C2%A0Navigate-to-the-Opportunities-Tab)  
   * [Step 2: Select What to Import](#Step-2%3A%C2%A0Select-What-to-Import)  
   * [Step 3: Upload Your CSV File](#Step-3%3A%C2%A0Upload-Your-CSV-File)  
   * [Step 4: Mapping Column to Fields](#Step-4%3A%C2%A0Mapping-Column-to-Fields)  
   * [Step 5: Verify, Confirm, and Finalize Selection](#Step-5%3A%C2%A0Verify,-Confirm,-and-Finalize-Selection)
* [Optional: Import Contacts & Opportunities](#Optional%3A-Import-Contacts-&-Opportunities)
* [Frequently Asked Questions](#Frequently-Asked-Questions)
* [Related Articles](#Related-Articles)

---

## **Prerequisites for Importing Contacts**

  
Before starting the import process, make sure you meet the following requirements:  
  
* User Permissions: Only users with Admin access can import contacts.
* File Format: The file must be in CSV (.csv) format.
* File Size Limit: The CSV file should be under 30 MB. If it's larger, split it into smaller files.
* Single Sheet Requirement: Your CSV file must contain only one sheet/tab.
* CSV Requirement: The first row should NOT be blank! Include a header row in which at least one column header corresponds to a field in the system.

---

## **Common Mistakes to Avoid**

  
❌ Mismatched headers: Ensure CSV headers match system fields.

  
❌ Blank required fields: Every row should have at least one required field (Name, Email, or Phone).

  
❌ Using special characters in phone numbers: Remove spaces, dashes, or letters.

  
❌ Duplicate records within CSV: Clean the list before importing.

---

## **Importing Opportunities via CSV** 

  
Importing opportunities allows you to bulk add or update deals in your HighLevel CRM. This streamlines data entry when onboarding clients or transitioning from another CRM, ensuring pipeline stages are aligned and sales activity is tracked accurately.

  
Efficiently managing opportunities through CSV imports helps keep your pipeline updated and your team aligned.

  
* **Save time:** Upload dozens or hundreds of opportunities in one go.
* **Maintain data accuracy:** Structured fields prevent common errors.
* **Improve consistency:** Ensure pipeline stages and values follow a standard.
* **Speed up onboarding:** Quickly integrate leads from previous systems.
* **Update existing deals:** Easily modify opportunity stages or values.
* **Sync contacts and opportunities:** Ensure opportunity data links directly to contact records.

---

## **How to Import Opportunities**

  
Importing opportunities involves a series of steps to ensure your sales data is accurately and efficiently entered into the CRM. From preparing your CSV file to mapping fields and confirming the import, this section walks you through everything you need to know to complete a successful import process. Follow these steps to successfully import opportunities into HighLevel using a CSV file.
  
  
### **Step 1:** Navigate to the Opportunities Tab

  
From the **Opportunities Tab**, click on the **Import** button to get started.

  
![](https://s3.amazonaws.com/cdn.freshdesk.com/data/helpdesk/attachments/production/155045398745/original/dmNghj-ZxoR9JhTKtXJ_qinPuZaG_v_tTw.png?1745246916)
  
  
### **Step 2:** Select What to Import

  
Choose whether you’re importing only Opportunities or both Contacts and Opportunities.

  
![](https://s3.amazonaws.com/cdn.freshdesk.com/data/helpdesk/attachments/production/155045398815/original/gB0nH9yhrsJcbDs1ccI61Se_uwwrNLUlkQ.png?1745247057)
  
  
### **Step 3:** Upload Your CSV File

  
After selecting to **Import Opportunities**, click Next, then upload your CSV file and select the correct import type depending on whether you’re adding new contacts or updating existing ones.

  
![](https://s3.amazonaws.com/cdn.freshdesk.com/data/helpdesk/attachments/production/155045398892/original/qm1aXwlk4hODcM2__8teU7ZgUUYUANY32w.gif?1745247178)
  
  
### **Step 4:** Mapping Column to Fields

  
Ensure each column in your file is correctly mapped to the corresponding field in the system. A few things to note:

  
1. Checking the "Don't update Empty Values" checkbox will not update any field if the imported file has empty values and the field does have some value for the opportunity.
2. If you decide not to import a certain field, you can choose to keep it unmapped and check the box on the bottom to proceed. -"Please ensure all mandatory fields are mapped. To proceed, either map all fields or choose Don't import data for unmapped columns."
3. If Contacts and Opportunities are on the same line in the CSV, they will be automatically mapped to each other.
4. Match your CSV columns to the required HighLevel fields:
* **Contact ID** (required)
* **Opportunity Name** (required)
* **Pipeline** (required)
* **Other fields**: Opportunity Value, Opportunity ID (if updating)

Mapped fields with correct values will show green checkmarks. If a field is missing or incorrect, a yellow warning triangle will appear.

  
![](https://s3.amazonaws.com/cdn.freshdesk.com/data/helpdesk/attachments/production/155045399088/original/i83vv5109onZK191E1UJ32Vt-Xa4dvoCew.gif?1745247525)
  
  
**Tip**: When all required fields are mapped successfully, all indicators will turn green.
  
  
### **Step 5:** Verify, Confirm, and Finalize Selection

  
Finalize the setup by reviewing your preferences, checking field mappings, and confirming consent before starting the import. This final step ensures that contacts are correctly tagged, sorted, and added to workflows, with your data fully verified. In the final step, you can:

  
* Add tags to imported contacts (optional)
* Review the document name and mapped fields
* Click **Start Bulk Import** to complete the process

  
Review your Field Mapping. Make sure all mandatory fields are correctly mapped. Confirm that custom fields are assigned as intended. Optional: Unmapped columns will be ignored automatically.

  
![](https://s3.amazonaws.com/cdn.freshdesk.com/data/helpdesk/attachments/production/155045399230/original/1FXu2Z7mvmnfEZkhLSHNqygn_K8_M9aPmQ.gif?1745247756)

---

## **Optional: Import Contacts & Opportunities**

  
If your CSV includes both contact and deal (opportunity) information, you can import both at once using the same flow. This is especially useful if you're onboarding new leads directly into your sales pipeline and want to associate them with a stage or deal value during the import. The process remains exactly the same as importing contacts, the only difference is selecting both "Contacts" and "Opportunities" during the initial import setup.

  
After clicking the **Import** button on the Contacts page, you’ll be prompted to select objects to import. Simply check both and proceed with the same steps as stated above.

  
## ![](https://s3.amazonaws.com/cdn.freshdesk.com/data/helpdesk/attachments/production/155045399289/original/ee7wjJSlhAu6H2VG-HVe8r8PAXJhpnsw2g.jpeg?1745247905)

---

**Frequently Asked Questions**

  
**Q: Can I import opportunities without contact data?**

No, each opportunity must be linked to a valid **Contact ID** in your account.
  
  
**Q: What file format is required?**

The file must be in **CSV format** (max 30MB).
  
  
**Q: Can I import opportunities into multiple pipelines?**

Yes, as long as the **Pipeline** name matches one that already exists in your account.
  
  
**Q: What happens if fields are mapped incorrectly?**

The import will fail or skip affected rows. Ensure all required fields are properly mapped and formatted.
  
  
**Q: Can I preview or undo an import?**

Imports cannot be undone. Always double-check your data before importing. You can review past imports in **Bulk Actions**.

---

## **Related Articles**

* [Importing Contacts Using a CSV File](https://help.gohighlevel.com/support/solutions/articles/155000004432-importing-contacts-using-a-csv-file)
* [CSV File Format for Importing Contacts and Opportunities](https://gohighlevelassist.freshdesk.com/support/solutions/articles/155000005143-csv-file-format-for-importing-contacts-and-opportunities)