**Date Updated:** 2024-08-21T21:40:40.000Z

**TABLE OF CONTENTS**

* [Overview](#Overview)
* [Trigger Name](#Trigger-Name)
* [Trigger Description](#Trigger-Description)
* [How to Configure](#How-to-Configure)
* [Example](#Example)

## Overview

The **New Signup** trigger is designed to automatically initiate workflows when a new customer signs up for a membership, service, or product. This trigger is particularly useful for welcoming new members, delivering onboarding information, or providing incentives for signing up.

  
## Trigger Name

**New Signup**

  
## Trigger Description

The **New Signup** trigger activates a workflow when a new customer signs up for an offer, membership, or any service you are providing. You can use this trigger to automate welcome emails, provide access to resources, or apply specific tags to the new customer’s profile.

  
## How to Configure

![](https://s3.amazonaws.com/cdn.freshdesk.com/data/helpdesk/attachments/production/155031250884/original/v4G0iHiP_bgAkWP9KjrgltVQ2btT3IfWRw.png?1724056828)

  
To configure the **New Signup** trigger, you need to define the workflow trigger name and set filters based on the offer or criteria you wish to monitor.

  
| Field                 | Description                                                                                 | Mandatory |
| --------------------- | ------------------------------------------------------------------------------------------- | --------- |
| Workflow Trigger Name | Name given to the trigger for easy identification.                                          | Yes       |
| Offer                 | Specify the offer that the new signup relates to (e.g., a discount or specific membership). | No        |
  
  
## Example

![](https://s3.amazonaws.com/cdn.freshdesk.com/data/helpdesk/attachments/production/155031251169/original/0AZYu07Mbu7vKdg7ewxA-oD4Uk3HzgvgeA.png?1724056969)

  
In this example, the workflow is set up to trigger when a customer signs up for a membership and selects the "15% Early Bird Discount" offer:

1. **Workflow Trigger Name:** Course` New Sign Up`
2. **Offer:** `15% Early Bird Discount`

####   

#### **Example Workflow**

When a customer signs up for a membership using the "15% Early Bird Discount" offer, the following actions could be triggered:

* **Send a Welcome Email:** Automatically send a personalized welcome email to the new member, outlining the next steps and providing relevant information.
* **Tag Customer:** Apply a tag such as "Early Bird" to the customer's profile for easy segmentation in future campaigns.

  
This configuration ensures that the workflow is triggered only when a customer signs up using the specific "15% Early Bird Discount" offer, allowing for targeted and relevant automated actions.