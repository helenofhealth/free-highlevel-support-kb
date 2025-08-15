**Date Updated:** 2024-09-17T14:55:05.000Z

**TABLE OF CONTENTS**

* [Overview](#Overview)
* [Action Name](#Action-Name)
* [Action Description](#Action-Description)
* [How to Configure](#How-to-Configure)
* [Example](#Example)

##   

## Overview

A one-time link is a unique scheduling link that automatically expires upon booking. With the 'Generate One-Time Booking Link' action, users can now effortlessly create these links directly within their workflow.

  
## Action Name

Generate One Time Booking Link

  
## Action Description

This action eliminates the manual effort involved in link creation, ensuring a seamless and error-free scheduling process. This action offers a dynamic, effective, and flexible approach to managing bookings, providing users with greater control and adaptability.

  
## How to Configure

To generate dynamic One-Time Links within your workflow, follow these simple steps:

  
**1\. Create a Workflow:** Start by creating a workflow in your account. Define the trigger that initiates the workflow based on your specific needs.

  
[![](https://s3.amazonaws.com/cdn.freshdesk.com/data/helpdesk/attachments/production/155032993277/original/O10E6elJz1v8jSs4umstCeXyk0Ax-gigpA.png?1726564861)](https://s3.amazonaws.com/cdn.freshdesk.com/data/helpdesk/attachments/production/155018179878/original/9PH-4QaDl1YRM4CRiWB2XUQGAMQ-z3B54w.png?1705662313)

  
**2\. Add the 'Generate One-Time Booking Link' Action:** Within your workflow, add an action. Navigate to the 'Appointments' category and select 'Generate One Time Booking Link.'

  
[![](https://s3.amazonaws.com/cdn.freshdesk.com/data/helpdesk/attachments/production/155032993274/original/r8Xt76pd0HYYErmU1OT6R31FJ204JTWmiw.png?1726564860)](https://s3.amazonaws.com/cdn.freshdesk.com/data/helpdesk/attachments/production/155018179038/original/YCkyI2w8TIZMetLj9EHdbrWc3tthBnU8FQ.png?1705662119)

**3\. Choose the calendar** for which you want to generate the one-time link.

[![](https://s3.amazonaws.com/cdn.freshdesk.com/data/helpdesk/attachments/production/155032993279/original/Pb-w18mPLnkVZA9Dd9tAKS0CfXj8JdU4dA.png?1726564861)](https://s3.amazonaws.com/cdn.freshdesk.com/data/helpdesk/attachments/production/155018180332/original/lDOQfOfeezXDE2rv93kRi7tuZRnssl3r0g.png?1705662475)

  
**4\. Share the Generated Link:** To share the link with your contact, add a communication action (e.g., email) to your workflow.

[![](https://s3.amazonaws.com/cdn.freshdesk.com/data/helpdesk/attachments/production/155032993278/original/HVn5xo9-tr9w71Eo6bQKLmBewFhjPc1FCg.png?1726564861)](https://s3.amazonaws.com/cdn.freshdesk.com/data/helpdesk/attachments/production/155018181091/original/RKQiBow9CoDlsPKjvyEGvC-0QiqzQ%5FJTHw.png?1705662726)

  
**5\. Add the Custom Value:** Insert the unique one-time link that will get generated each time a trigger is activated, into the email body using a custom value. Select 'Generate One Time Booking Link' and choose 'One Time Link.'

[![](https://s3.amazonaws.com/cdn.freshdesk.com/data/helpdesk/attachments/production/155032993280/original/CghJ2vb2XniMDcil1Gkh_Nf4_r2lAhvg7A.png?1726564861)](https://s3.amazonaws.com/cdn.freshdesk.com/data/helpdesk/attachments/production/155018180795/original/lGXO4iv2tvapxRKiIFiXIeulY%5F6LFexvVg.png?1705662663)

  
**6\. Customize Email Body:** Customize the email body as needed and click 'Save.'

  
**7\. Publish Workflow:** Once your workflow is set up, publish it. Now, each time a contact enters the workflow triggered by your defined condition, a unique one-time link will be generated and sent to them via email.

  
## Example

  
**Send a One Time Booking Link to a user who has submitted a Form**

  
**Trigger**

**Form Submitted** \- Add the trigger and select the form on submitting which the user should get a booking link.

  
**Action**

**Generate One time booking link** \- Add the action and select the Calendar.

**Send Email** \- In the email action, use custom value picker to add the One Time Booking Link in the email.

  
**Outcome**

As soon as a customer submits the form they will receive a booking link to your calendar and they can use that to schedule an appointment.