**Date Updated:** 2025-08-01T00:06:28.000Z

This article shows you how to add a custom wait time between cycles of a recurring countdown timer. Use the feature to run “Every Friday” flash sales, weekly webinar countdowns, or monthly product drops—without rebuilding timers each time they reset.

**TABLE OF CONTENTS**

* [What Is Custom Wait Time for Recurring Timers?](#What-Is-Custom-Wait-Time-for-Recurring-Timers?)
* [Key Benefits of Custom Wait Time](#Key-Benefits-of-Custom-Wait-Time)
* [How to Configure a Recurring Timer with Wait Time](#How-to-Configure-a-Recurring-Timer-with-Wait-Time)
* [Timer Lifecycle Explained](#Timer-Lifecycle-Explained)
* [Use-Case Templates](#Use-Case-Templates)
* [Known Behaviours & Tips](#Known-Behaviours-&-Tips)
* [Frequently Asked Questions](#Frequently-Asked-Questions)
* [Next Steps](#Next-Steps)

---

# What Is Custom Wait Time for Recurring Timers?

Custom wait time lets a recurring timer pause for a set duration after it reaches 00 : 00 : 00, then start the next cycle automatically. During the pause (the Wait state) you can decide whether the timer stays visible at zero or disappears entirely in funnels, while emails show a zero-state banner that links to your expiry page.

![](https://s3.amazonaws.com/cdn.freshdesk.com/data/helpdesk/attachments/production/155050757246/original/Zvnf4TGlWMr5O3hF3Tu93wuF8-EY-GqO5A.jpeg?1753986890)

## Key Benefits of Custom Wait Time

Adding a pause between cycles unlocks new campaign ideas and slashes repetitive setup work.

* Automate recurring promos such as “Every Friday Sale” or weekly challenges.
* Run evergreen webinars by counting down to the next session each week.
* Control visibility—hide timers in funnels during off-hours to keep pages tidy.
* Reuse a single asset across emails and funnels instead of cloning timers.
* Align email & page logic with consistent zero-state and redirect behaviour.

## How to Configure a Recurring Timer with Wait Time

Follow these steps once; the timer will self-manage every cycle.

1. Navigate to Marketing ▸ Countdown Timer ▸ New Timer.
2. Choose Recurring and set your Start and End offsets.
3. Toggle Custom Wait Time and enter a duration (e.g., 5 days 12 hours).
4. (Optional) Enable Hide Timer in Wait State to remove the timer from funnels during the pause.
5. Select the Expiry Page / URL visitors should see when they click the timer or refresh a funnel during Wait.
6. Save and embed the timer block in funnels and/or emails.

![](https://s3.amazonaws.com/cdn.freshdesk.com/data/helpdesk/attachments/production/155050757247/original/b9EMLlR4QylG8gEY_P4V8ww3-4L5dyefSg.jpeg?1753986890)

## Timer Lifecycle Explained

Knowing what contacts see at each stage helps you design seamless journeys.

vbnet

CopyEdit

Active Cycle ─┐

 │ hits 00:00

 ▼

 Wait State (custom duration)

 │ auto-restart

 ▼

 Next Active Cycle → … (repeats)

  
| State  | Email Behaviour                                                | Funnel Behaviour                                                                                                                              |
| ------ | -------------------------------------------------------------- | --------------------------------------------------------------------------------------------------------------------------------------------- |
| Active | Live ticking countdown                                         | Live ticking countdown                                                                                                                        |
| Wait   | Timer shows 00 : 00 : 00; clicking it redirects to Expiry Page | • Timer hidden or shows 00 : 00 : 00 (based on your toggle)• If the page is refreshed while Wait is active, user is redirected to Expiry Page |
| Reset  | New cycle begins automatically                                 | New cycle begins automatically                                                                                                                |

  
## Use-Case Templates

Plug-and-play numbers to hit the ground running.

| Scenario          | Start → End           | Wait Time     | Result                                        |
| ----------------- | --------------------- | ------------- | --------------------------------------------- |
| Every Friday Sale | Fri 00:00 → Fri 23:59 | 6 days 1 min  | Timer re-arms for the next Friday at midnight |
| Weekly Webinar    | Mon 09:00 → Thu 17:00 | 3 days 16 hrs | Countdown resumes each Monday morning         |
| Monthly Drop      | 1st 00:00 → 3rd 23:59 | 27 days       | Runs on the first three days of every month   |

  
## Known Behaviours & Tips

Avoid surprises by understanding edge-case logic.

* Email zero-state is unstyled “00 : 00 : 00”. Custom CSS/styling isn’t applied during Wait.
* Hide-Timer toggle affects funnels only; emails always show zero-state.
* If a visitor’s session spans Active → Wait without page refresh, they stay on the funnel page (no auto-redirect).
* Max wait duration: 365 days; Min: 1 minute.
* Analytics log a “Timer Expired” event the moment Wait starts—use it to trigger post-promo automations.

---

## Frequently Asked Questions

Q1\. Can a wait period cross Daylight-Saving-Time changes?  
 Yes—timers store durations, not fixed dates. The engine recalculates offsets when DST shifts.

Q2\. What happens if I edit the wait time later?  
 New duration applies the next time the timer enters Wait; the current cycle is unaffected.

Q3\. Can I style the zero-state in emails?  
 Not yet. Zero-state uses the default timer font and color for deliverability consistency.

Q4\. Does the redirect fire in funnels if I disable Hide-Timer?  
 Yes—refreshing the page during Wait always redirects, regardless of visibility.

Q5\. How many cycles can one timer run?  
 Unlimited—cycles continue until you archive or delete the timer.

Q6\. Will contacts see different times in cached emails?  
 Email timers refresh with real-time data when opened; cached images are replaced server-side.

Q7\. Can I add a wait period to non-recurring timers?  
 No—wait time is exclusive to the Recurring timer type.

---

### Next Steps

1. Build a pilot “Every Friday Sale” timer with a 7-day wait period.
2. Embed the timer block in a funnel landing page and preview the Wait-state behaviour.
3. Schedule an email blast using the same timer block.
4. Review analytics after two promo cycles and fine-tune your start/end offsets.
  
  