**Date Updated:** 2025-04-09T02:50:53.000Z

**TABLE OF CONTENTS**

* [Overview](#Overview)
* [Trigger Name](#Trigger-Name)
* [Trigger Description](#Trigger-Description)
* [How to Configure](#How-to-Configure)
* [Example](#Example)

##   

## **Overview**

  
This trigger initiates workflows when a viewer reaches a specified percentage of a video. It enables marketers to respond dynamically to viewer engagement levels, allowing for personalized follow-ups and targeted messaging based on how much of the video has been watched.

  
![](https://s3.amazonaws.com/cdn.freshdesk.com/data/helpdesk/attachments/production/155031420580/original/sXpACIXtpvOcK4StzPtPvJD4jvfsndNrMQ.png?1724242480)

## **Trigger Name**

Video Tracking

  
## **Trigger Description**

Runs when a lead watches upto a specified percentage of the video

  
**Please note:**   
The person watching the video should already be part of the CRM as contact for this trigger to work.
  
  
## **How to Configure**

  
Before you jump in to configure your trigger, we encourage you to go through this article - [Tracking Viewer Progress on a Funnel Hosted Video](https://help.gohighlevel.com/support/solutions/articles/48001227304-tracking-viewer-progress-on-a-funnel-hosted-video). 

1. **Prepare Your Video**:  
   * Ensure the video is properly encoded for tracking.  
   * Disable the progress bar in the video settings to ensure accurate tracking.  
   * Set Up a Redirect for Unregistered Visitors: Create a blank page with a form that captures visitor information before they can watch the video. This is crucial for tracking new users who may not be in your system yet.
2. **Create a New Workflow**:  
   1. Navigate to the workflow builder.
3. **Add the Video Tracking Trigger**:  
   1. Select the Video Event Tracking Trigger from the list of available triggers.  
   2. Set the specific percentage (e.g., 25%, 50%, 75%, or 100%) that will trigger the workflow.
4. **Define Actions**:  
   1. Add actions to the workflow, such as sending follow-up emails or SMS messages to viewers based on their engagement level.

**The video tracking trigger has 3 primary filters.** 

##   

| **Filter name**    | **Description**                                                                            | **Mandatory** |
| ------------------ | ------------------------------------------------------------------------------------------ | ------------- |
| Funnel             | The funnel in which the video is embedded                                                  | No            |
| Video              | The video for which you want to track the view percentage                                  | No            |
| Video Duration (%) | Set the specific percentage (e.g., 25%, 50%, 75%, or 100%) that will trigger the workflow. | No            |
  
  
![](https://s3.amazonaws.com/cdn.freshdesk.com/data/helpdesk/attachments/production/155031420924/original/uj1zHUqJwq32Dk81JaEjx2FlcGfKQX0Qbg.png?1724242714)
  
  
## Example

  
Here are some examples of how you can use the Video Event Tracking Workflow Trigger in:

  
## Example 1: Webinar Follow-ups

  
You host a webinar that includes a pre-recorded video presentation. Set up the following workflow:

* **Trigger**: Activate when a viewer watches 50% of the video.
* **Action**: Send a personalized email thanking them for watching and offering additional resources related to the content they viewed.
* **Trigger**: Activate when a viewer watches 100% of the video.
* **Action**: Send a different follow-up email inviting them to schedule a consultation or offering a special discount.

This workflow allows you to nurture leads based on their engagement level, providing relevant content and offers to increase the likelihood of conversion.

  
## Example 2: Lead Scoring

  
Assign points to viewers based on the percentage of the video they watch. Use these points for lead scoring and prioritization:

* **Trigger**: Activate when a viewer watches 25% of the video.
* **Action**: Add 10 points to their lead score.
* **Trigger**: Activate when a viewer watches 50% of the video.
* **Action**: Add an additional 20 points to their lead score.
* **Trigger**: Activate when a viewer watches 75% of the video.
* **Action**: Add 30 more points to their lead score.

By assigning higher points to viewers who watch more of the video, you can identify and prioritize the most engaged leads for targeted follow-ups and sales outreach.

  
## Example 3: Abandoned Video Tracking

  
Set up a workflow to track viewers who abandon the video before completion:

* **Trigger**: Activate when a viewer watches less than 50% of the video.
* **Action**: Add them to a segment for "Abandoned Video Viewers."
* **Action**: Send a follow-up email with a link to the video, encouraging them to complete it.

This workflow allows you to identify and re-engage viewers who may have been interested in your content but didn't complete the video for some reason. By sending a targeted follow-up, you can increase the chances of them finishing the video and taking further action.These examples demonstrate the versatility of the Video Event Tracking Workflow Trigger. By setting up targeted workflows based on viewer engagement, you can enhance lead generation, nurturing, and overall marketing effectiveness.

  
**FAQs**

  
* The trigger in workflows will when a user closes or completes the video.
* If no Video tracking % is added then the trigger will fire when the contact closes the window or completes the video (irrespective of the % watched)
* If you want to fire the trigger when user has watched at least 20% of the video change the operator to "Greater than or Equal to" instead of "Equals to
* The workflows will get the data every time the user closes the video, so if the user revisits the page and fulfils all the requirements mentioned in the filter it will re-enter if Allow Re-entry is turned on
  
  