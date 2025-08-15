**Date Updated:** 2025-04-22T01:22:51.000Z

This article will help you identify why specific appointment timeslots are either not showing when they should, or appearing when they shouldn't on your HighLevel calendar. Whether you're using a standard or round robin calendar, we'll walk you through the most common causes and how to fix them—so you can get back to booking smoothly!

---

**TABLE OF CONTENTS**

* [What is Time Slot Visibility in HighLevel?](#What-is-Time-Slot-Visibility-in-HighLevel?)
* [Key Benefits of Understanding Time Slot Visibility](#Key-Benefits-of-Understanding-Time-Slot-Visibility)
* [How to Troubleshoot Missing or Unexpected Time Slots](#How-to-Troubleshoot-Missing-or-Unexpected-Time-Slots)  
   * [Calendar Settings](#Calendar-Settings)  
   * [Slot Duration, Buffers & Interval Settings](#Slot-Duration,-Buffers-&-Interval-Settings)  
   * [External Conflicts & Calendar Sync](#External-Conflicts-&-Calendar-Sync)  
   * [Timezones](#Timezones)  
   * [Use the Calendar Troubleshooting Tool](#Use-the-Calendar-Troubleshooting-Tool)
* [Frequently Asked Questions](#Frequently-Asked-Questions)
* [Related Articles](#Related-Articles)

---

  
---

# **What is Time Slot Visibility in HighLevel?**

  
Time slot visibility refers to whether or not appointment booking slots appear to your clients on your public calendar. These slots are determined by a combination of factors—calendar settings, user availability, buffer times, external conflicts, and Round Robin logic. When something’s misconfigured, you may run into issues like:

  
* A user is available but their time slots are missing
* Time ranges are open but not bookable
* The calendar shows more (or fewer) times than expected

Understanding how these variables interact is essential to diagnosing the issue.

---

## **Key Benefits of Understanding Time Slot Visibility**

  
Knowing how calendar logic works helps you reduce missed bookings, improve user experience, and troubleshoot faster.  
  
* Identify configuration issues faster
* Avoid overlapping or conflicting calendar events
* Optimize team availability with correct Round Robin settings
* Use the built-in Troubleshooting Tool for deeper insights
* Minimize client friction during booking

---

  
## **How to Troubleshoot Missing or Unexpected Time Slots**

  
Time slot issues can result from multiple overlapping factors. Use the grouped checklist below to methodically diagnose and correct visibility problems.

  
## **Calendar Settings**

  
Calendar configurations are the foundation of availability logic. Incorrect selections here are a common cause of visibility issues.

  
### **Check that you're viewing the correct calendar.**

  
Go to **Calendars > Calendar Settings**. Click **Edit** on desired calendar. Confirm you are working inside the intended calendar by checking calendar name, calendar group and calendar type.  
  
![](https://s3.amazonaws.com/cdn.freshdesk.com/data/helpdesk/attachments/production/155045405263/original/loQj-3YHxK0hML3pP8EQUMyLcg_IALW1qg.png?1745261533)  
  
### **Verify working hours and custom date availability**

  
Click **Edit** on the desired calendar. Visit the calendar's **Availability** tab and confirm that:

  
* Weekly hours are properly set.
* Date-specific overrides haven’t blocked times. Learn more about availability settings.

  
![](https://s3.amazonaws.com/cdn.freshdesk.com/data/helpdesk/attachments/production/155045405187/original/i-l7v9Nqp5UDMFb5Ypipb_Ynm2iGkM2tpw.png?1745261299)
  
  
### **Confirm the correct user(s) or team is assigned**

  
Availability is based on the assigned users. Check under Team Members Assigned by clicking edit on desired calendar then using the dropdown named **Select** **Te** **am Member & Assign Meeting Location** in the Service Details tab.

  
![](https://s3.amazonaws.com/cdn.freshdesk.com/data/helpdesk/attachments/production/155045405140/original/Jmt8EbsjGJjmCovw7-ljQJdfuoj5xUNcSA.png?1745261152)

---

## **Slot Duration, Buffers & Interval Settings**

  
How your slots are spaced—and buffered—can create gaps or block slots entirely.  
  
### **Check your slot interval, duration and buffer settings.**

  
These control how often time slots appear and how long they are. To edit, Go to **Settings** → **Calendars**. Click on the calendar you want to edit. In the calendar editor, navigate to the **A** **vailability** tab. Scroll to the **Slot Duration, Post Buffer Time** and **Slot Interval** fields and adjust the values to match your service needs.

  
### ![](https://s3.amazonaws.com/cdn.freshdesk.com/data/helpdesk/attachments/production/155045405376/original/TWzMT4XREii7qQZxOktc_FK_YS-60ACebg.png?1745261927)

---

## **External Conflicts & Calendar Sync**

  
Connected calendars can block availability based on busy times. Check for events blocking slots in synced Google/Outlook calendars.  
  
External calendar events—if marked busy—will block slots on the internal calendar. [Learn more on how conflicts work](https://help.gohighlevel.com/en/support/solutions/articles/155000002374)

---

## **Timezones**

  
Timezone mismatches are a hidden but common issue, especially across teams or international clients.

  
### **Make sure all timezones align**

  
Double-check both your user profile settings and the client’s calendar view to make sure A 3 PM slot for one user could be 10 AM for another.

---

## **Use the Calendar Troubleshooting Tool**

  
### **Use the Troubleshooting Tool to understand slot logic**

  
This built-in feature breaks down exactly why a time slot is blocked. To access the tool, Navigate to Calendar Settings, locate the calendar you want to troubleshoot, and select Troubleshoot Calendar (Wrench Icon). [Learn More on how to use the Calendar Troubleshooting Tool](https://help.gohighlevel.com/en/support/solutions/articles/155000003358)  
  
**![](https://s3.amazonaws.com/cdn.freshdesk.com/data/helpdesk/attachments/production/155045405564/original/-YIahFFfZNQu-2uvvTxD2crSnSy1z1G-dw.png?1745262428)**

---

## **Frequently Asked Questions**

  
**Q: Why does a team member show available but isn’t getting booked?**  
The Round Robin logic may be skipping them due to prior assignments or availability priority settings.

**Q: Why are my booking slots not aligning with my working hours?**  
This could be due to slot intervals, buffer times, or hidden external calendar conflicts.

  
**Q: Why do slots show up on some browsers but not others?**  
Browser caching or mismatched timezone display can cause these inconsistencies.

  
**Q: Can I allow clients to pick their preferred team member?**  
Yes, enable **staff selection** under the calendar’s settings if you're using Round Robin.

  
**Q: What does the troubleshooting tool show me?**  
It lists every rule or condition blocking a specific slot, including time zone, buffer, user assignment, and more.

---

## **Related Articles**

  
* [Round Robin Calendars: The Setup Guide](https://help.gohighlevel.com/en/support/solutions/articles/155000001485)
* [Troubleshooting Tool for Calendar](https://help.gohighlevel.com/en/support/solutions/articles/155000003358)
* [Adjusting Availability Settings](https://help.gohighlevel.com/en/support/solutions/articles/48001155718)
* [Pre and Post Buffers](https://help.gohighlevel.com/en/support/solutions/articles/155000001019)
* [Calendar Scheduling Conflicts](https://help.gohighlevel.com/en/support/solutions/articles/155000003548)
* A[ppointment Distribution Logic](https://help.gohighlevel.com/en/support/solutions/articles/155000001484)