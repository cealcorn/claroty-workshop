---
title: "Events vs. Alerts vs. Stories"
description: ""
---
## GOALS
- Understand the difference between events, alerts, stories, security events, and process integrity alerts
---
## TASKS
### Part One: Events
1. Navigate to `Threat Detection` > `Events` and review the Events page.
2. Note:
   - Total number of events
   - Type of events
   - Status of events
   - Dates detected
3. Choose an event by clicking on its ID, open it, and review the name, the type of event, the policy violations, and when it was generated.
4. From the Event details page, identify any related assets, policies, alerts, or navigation links that can be used to investigate the event further.
### Part Two: Alerts
1. Go to `Threat Detection` > `Alerts` and review the Alerts page.
2. Like the events, review the page and determine the number, type, status, and time of the listed alerts. You can also switch between views.
3. Choose an alert, open it, and review:
   - Alert Type
   - Severity
   - Status
   - Associated Assets
   - Description
4. If possible, attempt to find an alert that is correlated with the Event you previously investigated.
5. Navigate from the alert to any associated assets and review the additional context available.
> The sensitivity of alerts can be adjusted by going to `Settings` > `Alerts` > `Alert Sensitivity`.
### Part Three: Stories
1. Go to `Threat Detection` > `Alerts`.
2. Enable `Group by Story`, located in the top right of the web page.
2. Select a story and review:
   - Story ID
   - Status
   - Number of Alerts
   - Assets Involved
   - Date Range
5. Expand the story and review the alerts contained within it.
6. Open at least one alert from the story and compare its information to the story view.
7. Determine:
   - Which alert appears most significant?
   - How many assets are involved?
   - Whether the story appears to describe a single activity or multiple related activities.
8. Return to the Alerts page and disable Group by Story.
9. Locate one of the alerts that was previously contained within the story.
10. Compare the information available when viewing:
    - The Alert individually
    - The Alert as part of a Story
---
## REFLECTION
- What do events, alerts, and stories represent?
- Does every event appear malicious? Could normal activities generate events?
- How does an alert differ from an event? What information does it provide that events do not?
- How do stories differ from alerts? What information do they provide that alerts alone do not?
- Why do you think CTD provides all three, and what information would be lost if each one did not exist?
