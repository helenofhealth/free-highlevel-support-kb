**Date Updated:** 2025-07-23T19:40:21.000Z
  
  
Importing contacts and opportunities in bulk using a CSV file is an essential feature in HighLevel that helps streamline data entry and organization. You can map fields, create or update records, and monitor the import process seamlessly, ensuring accurate data entry and time-saving for bulk actions. This guide provides a step-by-step walkthrough, from preparing your CSV file to monitoring the import process and fixing errors.

  
**TABLE OF CONTENTS**

* [Prerequisites for Importing Contacts and Opportunities](#Prerequisites-for-Importing-Contacts-and-Opportunities)
* [Common Mistakes to Avoid](#Common-Mistakes-to-Avoid)
* [Importing Contacts and Opportunities](#Importing-Contacts-and-Opportunities)  
   * [Choose What To Import](#Choose-What-To-Import)  
   * [Upload Your CSV File](#Upload-Your-CSV-File)  
   * [Mapping Column to Fields](#Mapping-Column-to-Fields)  
   * [Reviewing and Completing the Import](#Reviewing-and-Completing-the-Import)
* [Monitor Import Status](#Monitor-Import-Status)
* [Frequently Asked Questions](#Frequently-Asked-Questions)
* [Related Articles](#Related-Articles)

---

## **Prerequisites for Importing Contacts and Opportunities**

  
Before starting the import process, make sure you meet the following requirements:  
  
* **User Permissions:** Only users with **Admin** access can import contacts.
* **File Format:** The file must be in **CSV (.csv) format**.
* **File Size Limit:** The CSV file should be **under 30MB**. If it's larger, split it into smaller files.
* **Single Sheet Requirement:** Your CSV file must contain **only one sheet/tab**.
* **CSV Requirement**: The first row should **NOT** be blank! Include a header row in which at least one column header corresponds to a field in the system.

---

## **Common Mistakes to Avoid**

  
❌ **Mismatched headers**: Ensure CSV headers match system fields.

  
❌ **Blank required fields**: Every row should have at least one required field (Name, Email, or Phone).

  
❌ **Using special characters in phone numbers**: Remove spaces, dashes, or letters.

  
❌ **Duplicate records within CSV**: Clean the list before importing.

---

## **Importing Contacts and Opportunities**

  
There are two ways to access the Import Contacts and Opportunities feature in HighLevel.  
  
1. From within the **Contacts Tab**  
   * Navigate to Contacts from the left-hand menu, click on the Smart Lists tab, and click the Import Contacts button.  
         
   ![](https://s3.amazonaws.com/cdn.freshdesk.com/data/helpdesk/attachments/production/155040930961/original/yW_9vq1gWBiCtPOzzi2VJmvf6boUSaN6zg.jpeg?1738599031)
2. From within the **Opportunities Tab**  
   * Navigate to Opportunities from the left-hand menu, then Click the Import button in the top-right corner.  
         
   ![](https://s3.amazonaws.com/cdn.freshdesk.com/data/helpdesk/attachments/production/155040930986/original/8MqKQhBikQMrYyLxrl1XnGtTPblojpxx-A.jpeg?1738599048)

####   

  
Both methods lead to the same import process, where you can choose to import:  
1. Contacts  
2. Opportunities  
3. Both Contacts & Opportunities at the same time
  
  
### **Choose What To Import**
  
  
![](https://s3.amazonaws.com/cdn.freshdesk.com/data/helpdesk/attachments/production/155040931304/original/whSQMNJr1Gf3poHw2aHt68bxBwKX_wElsA.jpeg?1738599293)
  
  
### **Upload Your CSV File**

  
**Step 1**: After selecting to import Contacts, Opportunities, or both, click Next, then click Upload File and choose your CSV file from your computer.

  
![](https://s3.amazonaws.com/cdn.freshdesk.com/data/helpdesk/attachments/production/155040673232/original/U6Ezequ3JHtmkRbRUYlCdowbOAOFPlw1RA.gif?1738168901)
  
  
**Step 2**: Upload the file for importing and then click on "Choose how to import contacts/opportunities" to decide whether you want to create, update, or do both.

  
![](https://s3.amazonaws.com/cdn.freshdesk.com/data/helpdesk/attachments/production/155040673389/original/1wbH4t9zwC4jss4xrDWDyMQBGScc9oeYnw.png?1738169062)
  
  
**Please Note**: Find existing contacts based on Filter by default is set to email ,then phone, which means, Contacts/Opportunities would be filtered by email first and if email not found then phone.
  
  
### **Mapping Column to Fields**

  
Ensure each column in your file is correctly mapped to the corresponding field in the system.

A few things to note:

1. Checking the "Don't update Empty Values" checkbox will not update any field if the imported file has empty values and the field does have some value for the opportunity.
2. If you decide to not import a certain field, you can choose to keep it unmapped and check the box on the bottom to proceed. -"Please ensure all mandatory fields are mapped. To proceed, either map all fields or choose Don't import data for unmapped columns"
3. This feature also allows the creation of **contacts** with multiple email addresses and phone numbers. These additional details will be added automatically during the import process.
4. If Contacts and Opportunities are on the same line in the CSV, they will be automatically mapped to each other.

  
![](https://s3.amazonaws.com/cdn.freshdesk.com/data/helpdesk/attachments/production/155040673955/original/qTkj_KxMtSIGVm4td90AiKIauWMgpKBRkg.png?1738169641)
  
  
### **Reviewing and Completing the Import**

  
Review your mappings, then confirm and proceed with the import, you can also choose to **C** **reate a Smart list**, add contacts to a **Workflow**, or add a new **Tag** to the imported contacts.

  
Create a Smartlist from Imports  
Adding contacts to workflows

  
![](https://s3.amazonaws.com/cdn.freshdesk.com/data/helpdesk/attachments/production/155040674777/original/UqeVsoGa1tluVwGM-OxyGzXk4dgiADAj_Q.png?1738170432)
  
  
It is mandatory to select the checkbox confirming all the contacts/opportunities for import.

---

## **Monitor Import Status**

  
* You can monitor the progress and status of the import via the Contacts and Opportunities **Bulk Actions** Pages.
* Both contacts and opportunities imports will appear in the same place under **Bulk Actions.**
* Click on the "**Show Stats**" button to view the Stats of the import - you can also download the error log and view further details about the error and how to fix them in the "**Error**" tab

  
![](https://s3.amazonaws.com/cdn.freshdesk.com/data/helpdesk/attachments/production/155040675205/original/9137ojlvH-YH7-gdZ0MwQa2zapRtYwe4kg.gif?1738170977)
  
  
The phone field from the CSV export in Keap is incompatible with GHL. The parenthesis '()' and dashes '-' make it incompatible. We have to highlight the entire column in the CSV file and ensure it is numbered in, remove any parenthesis and dashes, and then we can import without corrupting the data in the CRM.

---

## **Frequently Asked Questions**

  
Q. What happens if my CSV file is over 50MB?

Split the file into **smaller sections (under 50MB)** and import them separately.

  
Q. Can I import contacts with multiple emails or phone numbers?

Yes! Additional emails and phone numbers are stored **as secondary fields** instead of replacing primary data.

  
Q. How does HighLevel handle duplicate contacts?

* **HighLevel automatically merges** contacts based on phone number or email.
* If a match is found, the system **updates existing records** instead of creating duplicates.

  
Q. Can I update existing contacts via CSV import?

Yes! Choose **Update Only** or **Create & Update** during import.

  
Q. What should I do if my import fails?

* Check **error messages** in the **Import Status Page**.
* Download the **error log**, fix the issue, and **re-import the corrected CSV**

Q: Why are all my imported contacts set to DND for ALL channels? How can I apply DND for specific channels only?

When importing contacts with a **DND (Do Not Disturb) column** in your CSV, HighLevel **automatically applies DND for all communication channels** (SMS, Email, Calls, Voicemail, etc.).

If you want to set **DND for specific channels only**, you need to use a **workflow and tags** instead of the DND column.

  
Q. I'm trying to import a CSV with Notes, and I cannot generate more than one note per contact record.

When importing contact notes, you may only have one note per contact record with a limit of **5000** **characters**.

---

## **Related Articles**

* **[](https://help.gohighlevel.com/support/solutions/articles/155000004432-importing-contacts)**[](https://help.gohighlevel.com/support/solutions/articles/155000004432-importing-contacts)[Importing Contacts](https://help.gohighlevel.com/support/solutions/articles/155000004432-importing-contacts)[](https://help.gohighlevel.com/support/solutions/articles/155000004432-importing-contacts)**[](https://help.gohighlevel.com/support/solutions/articles/155000004432-importing-contacts)**
* **[](https://help.gohighlevel.com/support/solutions/articles/48001181714-allow-duplicate-contact-explained)**[](https://help.gohighlevel.com/support/solutions/articles/48001181714-allow-duplicate-contact-explained)[Allow Duplicate Contact Explained](https://help.gohighlevel.com/support/solutions/articles/48001181714-allow-duplicate-contact-explained)[](https://help.gohighlevel.com/support/solutions/articles/48001181714-allow-duplicate-contact-explained)**[](https://help.gohighlevel.com/support/solutions/articles/48001181714-allow-duplicate-contact-explained)**