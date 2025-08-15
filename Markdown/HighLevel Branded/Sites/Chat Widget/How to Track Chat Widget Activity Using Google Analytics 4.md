**Date Updated:** 2025-05-29T18:15:30.000Z

This article provides guidance on integrating HighLevel's Chat Widget with Google Analytics 4 to monitor user interactions effectively across funnel steps, website pages, Wordpress websites and any other integration like Shopify, Wix or Squarespace. 

---

**TABLE OF CONTENTS**

* [What is Chat Widget GA4 Tracking?](#What-is-Chat-Widget-GA4-Tracking?)
* [Key Benefits of GA4 Tracking for Chat Widget](#Key-Benefits-of-GA4-Tracking-for-Chat-Widget)
* [Integrate Chat Widget with GA4 Tracking](#Integrate-Chat-Widget-with-GA4-Tracking)
* [GA4 Tracking Events Captured by the Chat Widget](#GA4-Tracking-Events-Captured-by-the-Chat-Widget)
* [Frequently Asked Questions](#Frequently-Asked-Questions)
* [Related Articles](#Related-Articles)

---

# **What is Chat Widget GA4 Tracking?**

  
HighLevel's Chat Widget can be embedded across various platforms, including funnels, websites, and WordPress sites. By integrating GA4 (Google Analytics), you can track user interactions with the Chat Widget, enabling better insights into user behavior and engagement.

---

## **Key Benefits of GA4 Tracking for Chat Widget**

* **Enhanced User Insights**: Monitor how users interact with the Chat Widget to optimize engagement strategies.
* **Performance Monitoring**: Identify and address potential issues in the chat experience.
* **Data-Driven Decisions**: Leverage analytics to make informed decisions about chat functionalities.
* **Seamless Integration**: Combine Chat Widget and GA4 scripts without conflicts.

---

## **Integrate Chat Widget with GA4 Tracking**

  
Make sure Google Analytics 4 (GA4) is already installed on the site or funnel where your Chat Widget will appear. No additional configuration is required for the Chat Widget to send events to GA4.  
  
* This applies to all platforms — including HighLevel sites, funnels, WordPress, Wix, Shopify, and others.
* You do not need to install GA4 separately for the widget to work.

  
Follow this structured setup to install GA4 tracking, embed the chat widget, and begin capturing custom analytics events related to widget usage.

  
### **1\. Add GA4 Global Site Tag**

Embed the following code in the <head> section of your webpage or in a GTM Custom HTML tag.

```html
<!-- Google Analytics 4 Global Site Tag -->
<script async src="https://www.googletagmanager.com/gtag/js?id=your-GA-code"></script>
<script>
  window.dataLayer = window.dataLayer || [];
  function gtag(){dataLayer.push(arguments);}
  gtag('js', new Date());
  gtag('config', 'your-GA-code');
</script>
```

HTML

Key Notes:

* This script loads the GA4 library and initializes it using your GA4 measurement ID: your-GA-code.
* dataLayer is used for storing events and sending them to GA4.

### **2\. Embed the Chat Widget**

Insert this snippet in the <body> section of your site to load the chat widget.

```html
<!-- Chat Widget Embed →
COPY THE CODE FROM THE SUB-ACCOUNT FOR GOOGLE TAG MANAGER (GTM)
<div
  data-chat-widget
  data-widget-id="widget-id"
  data-location-id="location-id">
</div>
<script
  src="https://widgets.leadconnectorhq.com/loader.js"
  data-resources-url="https://widgets.leadconnectorhq.com/chat-widget/loader.js"
  data-widget-id="widget-id">
</script>
```

HTML

Click on the "Get Code" button, then navigate to "Via GTM" section to find this snippet.![](https://s3.amazonaws.com/cdn.freshdesk.com/data/helpdesk/attachments/production/155047390964/original/wGXYrIMAkpOB10M7HGPU7l97_S-Zyds_4A.png?1748459488)

  
Attributes Breakdown:

* data-widget-id: Unique identifier for the widget.
* data-location-id: Corresponds to your business/location.

### **3\. Add GA4 Custom Event Tracking Script**

Paste this script below your chat widget embed to enable event tracking for widget interactions.

```html
<script>
  function trackGAEvent(eventName, label) {
    gtag('event', eventName, {
      event_category: 'Chat',
      event_label: label
    });
  }

  function beforeSubmit(values, host) {
    trackGAEvent('form-submit', 'Form Submitted');
    return true;
  }

  window.addEventListener("LC_chatWidgetLoaded", function (e) {
    var observer = new MutationObserver(function () {
      if (leadConnector.chatWidget.isActive()) {
        trackGAEvent('widget-open', 'Widget Open');
      } else {
        trackGAEvent('widget-close', 'Widget Close');
      }
    });
    observer.observe(e.detail, { attributes: true });
    window.leadConnector.chatWidget.registerBeforeSubmit(beforeSubmit);
  }, false);
</script>
```

HTML

---

## **Event Reference for GA4**

  
Understanding what each event tracks helps you validate and use the data more effectively in GA4.

  
| **Event Name** | **Trigger Condition**         | **Category** | **Label**      |
| -------------- | ----------------------------- | ------------ | -------------- |
| widget-open    | When the widget is opened     | Live Chat    | Widget Open    |
| widget-close   | When the widget is closed     | Live Chat    | Widget Close   |
| form-submit    | When a chat form is submitted | Live Chat    | Form Submitted |

  
---

## **Testing & Debugging Tips**

  
Use these techniques to confirm your event tracking is correctly set up and working in real time.

1. **Google Tag Assistant Extension**: Monitor events as you interact with the widget.
2. **GA4 DebugView**: Track real-time events in your Google Analytics dashboard.
3. **Network Logs**: Use browser DevTools → Network tab to verify event payloads.
4. **Live Test**: Open, close, and submit the chat form to validate the respective events.

---

## **Frequently Asked Questions**

**Q: Will this track users across all pages?** 
**Yes, as long as the widget and tracking script are embedded on those pages.** 
  
**Q: Can I customize the events tracked by the Chat Widget?** 
**Currently, the Chat Widget tracks a predefined set of events. Custom event tracking is not supported.** 
  
**Q: Where can I view the Chat Widget events in GA4?** 
**Navigate to the "Events" section in your GA4 property to view the tracked Chat Widget events.**

---

## **Related Articles**

* **[](https://help.gohighlevel.com/en/support/solutions/articles/48000984860) [](https://help.gohighlevel.com/en/support/solutions/articles/48000984860)[How to Install HighLevel's Chat Widget](https://help.gohighlevel.com/en/support/solutions/articles/48000984860)**
* **[Google Analytics 4 Tracking](https://help.gohighlevel.com/en/support/solutions/articles/48001234199)**
* **[Getting Started with Chat Widget](https://help.gohighlevel.com/en/support/solutions/articles/155000004102) [](https://help.gohighlevel.com/en/support/solutions/articles/155000004102)[](https://help.gohighlevel.com/en/support/solutions/articles/155000004102)**