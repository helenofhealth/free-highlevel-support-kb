**Date Updated:** 2024-01-16T16:19:37.000Z

With the Date/Time Formatter action, you can reformat the Date or Date and Time as per your requirement. You can also compare dates using the action.
  
  
**TABLE OF CONTENTS**

  
* Format Date
* Format Date and Time
* Compare Dates

  
![](https://s3.amazonaws.com/cdn.freshdesk.com/data/helpdesk/attachments/production/48293485600/original/mQC3q6W5GkDW_Um06RXgC_HIQuOXyamprA.png?1681915820)

  
---

## **How to Format a Date**

### To convert date structure from one format to another.  
  
**Field:**

Select any date field. You can select a Specific Date, or Current Date, from Contact's date fields or date type custom fields, Appointment start/end date, Custom values, or even Inbound Webhook Trigger.  
  
### ![](https://s3.amazonaws.com/cdn.freshdesk.com/data/helpdesk/attachments/production/48293499588/original/_1utIHUqHXOqAPs92BiTwpZww4BQsBrujQ.png?1681918643)
  
  
**From Format:**

Selecting system fields like Specific Date, Current Date, from Contact's date type standard fields, Contact's date type custom fields, or Appointment start or end date will auto-detect the format and preselect the same. If it is a Custom Value or from an Inbound Webhook trigger, you will have to select the exact matching format.

  
#### ![](https://s3.amazonaws.com/cdn.freshdesk.com/data/helpdesk/attachments/production/48293500391/original/1Kd6PUZXtT4AOQFWbBLkT2LOImgrmYP82g.png?1681918843)

####   
  
### **To Format:**

#### Select the required format from the list

![](https://s3.amazonaws.com/cdn.freshdesk.com/data/helpdesk/attachments/production/48293500697/original/Dlds7-wpcq09sncoJ5Yj3LJkGMkityYRNw.png?1681918918)
  
  
###   
**Output**

#### After setting up the Format Date, you can use the results in further actions in your Workflow {{datetime\_formatter.1.date}}

####   
Custom Values

### ![](https://s3.amazonaws.com/cdn.freshdesk.com/data/helpdesk/attachments/production/48293485199/original/i57GTs9YqhKeBH6jHV9SZ8b70o9BHxFqhA.png?1681915720)
  
  
---

## **Format Date and Time**

To convert date and time structure from one format to another

###   
**Field:**

Select any date-time field; you can select a Specific Date and Time, Current Date and Time, Appointment start or end date time, Custom values, or even from Inbound Webhook Trigger.

**Please note:**

Currently, Contact Custom fields do not support the Date Time structure.

  
![](https://s3.amazonaws.com/cdn.freshdesk.com/data/helpdesk/attachments/production/48293501865/original/vobWnYp1Evzld6XXk5ZHrhnEfHKOqONeag.png?1681919224)

  
###   
**From Format:**

Selecting any system fields like Specific Date and Time, Current Date and Time, Contact fields, or Appointment start or end date time will auto-detect the format and preselect the same. If it is a Custom Value or from an Inbound Webhook trigger, you will have to select the exact matching format.

  
![](https://s3.amazonaws.com/cdn.freshdesk.com/data/helpdesk/attachments/production/48293485200/original/ADCn7ZI9KM1XNRCewnqcX2MQFhLod3cGOA.png?1681915720)

####   

####   

###   
**To Format:**

Select the required format from the list

![](https://s3.amazonaws.com/cdn.freshdesk.com/data/helpdesk/attachments/production/48293502392/original/Hx6KmKS9a_LsIT3YPR28n1I5snd_5T-VHQ.png?1681919362)
  
  
### **Output**

After setting up the Format Date and Time, you can use the results in further actions in your Workflow.

{{datetime\_formatter.1.datetime}}

  
Custom Values

![](https://s3.amazonaws.com/cdn.freshdesk.com/data/helpdesk/attachments/production/48293502719/original/RafxrtJSJwOrKgFMTiiXu_QDJ3l8oFEzQQ.png?1681919449)  
  
  
##   

---

## **Compare Dates**

Compare two dates and get the difference in the number of days

###   
**Start Date:**

Select any date field. You can select a Specific Date, or Current Date, from Contact's date fields or date type custom fields, Appointment start/end date, Custom values, or even from Inbound Webhook Trigger.

![](https://s3.amazonaws.com/cdn.freshdesk.com/data/helpdesk/attachments/production/48293485206/original/pu4iIap9Yhth5gOEcLZ9F3bCAtyj-bLduw.png?1681915721)

####   

### **Start Date Format:**

Selecting system fields like Specific Date, Current Date, from Contact's date type standard fields, Contact's date type custom fields, or Appointment start or end date will auto-detect the format and preselect the same. If it is a Custom Value or from an Inbound Webhook trigger, you will have to select the exact matching format.  
  
![](https://s3.amazonaws.com/cdn.freshdesk.com/data/helpdesk/attachments/production/48293485196/original/x1alZjEhaa3Bcvql1AKt9urx0eoKr9Iu1A.png?1681915720)
  
  
### **End Date:**

Select any date field. You can select a Specific Date or Current Date from Contact's date fields or date type custom fields, Appointment start/end date, Custom values, or even an Inbound Webhook Trigger.

![](https://s3.amazonaws.com/cdn.freshdesk.com/data/helpdesk/attachments/production/48293485191/original/c1isR7MZKKuBytIQEFfAeVzdZHE0ST9idw.png?1681915720)
  
  
#### **End Date Format:**

Selecting system fields like Specific Date, Current Date, from Contact's date type standard fields, Contact's date type custom fields, or Appointment start or end date will auto-detect the format and preselect the same. If it is a Custom Value or from an Inbound Webhook trigger, you will have to select the exact matching format.

  
![](https://s3.amazonaws.com/cdn.freshdesk.com/data/helpdesk/attachments/production/48293485194/original/ms1zccoNhkzIk47RIxyB0Im3qaF2PHsP-w.png?1681915720)

####   

### **Output**

After setting up the Compare Dates, you can use the results in further actions in your Workflow. {{datetime\_formatter.1.days}}

  
The difference is calculated as End Date - Start Date, so you will get a negative value if the Start Date is greater than the End Date.

Custom Values

![](https://s3.amazonaws.com/cdn.freshdesk.com/data/helpdesk/attachments/production/48293485195/original/TQD4-jxcpOu4EmXENgwAN5WSqddc-uaBag.png?1681915720)

---

## **Usage**

* Format the Inbound Webhook Trigger data to Set Event Start Date, to update Contact Custom Fields, to compare in If/Else Condition.
* Let's say the date format is MM/DD/YYYY, but you need to send it to an app that formats dates as DD/MM/YYYY. You can use the Date/Time Formater to change the date format and send it via Custom Webhook.
* Store the custom formatted date time info in Google Sheets
* Use the custom formatted date time info in Email/SMS/Slack
* Compare the Current date(Start Date) with the Invoice Due date(End Date) and use the dynamic value in Email/SMS/Slack,  
Eg: Your Invoice is due in {{datetime\_formatter.1.days}} days,  
    
**Please Note:**

On overdue, that is when Current Date(Start Date) is greater than the Invoice Due Date(End Date) you will get the result in a negative value

  