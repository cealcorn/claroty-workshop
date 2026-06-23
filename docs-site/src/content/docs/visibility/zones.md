---
title: "Visibility: Zones"
description: "✅"
---
We have broadly reviewed the network (via **Overview**) and began to explore specific assets (via **Assets**). 

Our next step is to determine how specific assets communicate amongst themselves. The first part of this understanding is to group assets, such as by function (e.g. "HMIs") or communication protocols ("HVAC systems speaking BACnet").

We will want to:
* Determine how many zones are in the environment
* Determine the attributes of existing zones (population, criticality, etc.)
* Determine which zones are in communication with other zones
* Understand how zones can be used to determine what assets may pose a higher risk than others

---

## TASKS

1. Navigate to `Visibility` > `Zones`.
<br/><br/>
2. Review the list of zones.
<br/><br/>
3. Examine:
   - The number of assets in each zone,
   - The risk level of each zone,
   - And the criticality of each zone.
<br/><br/>
4. Switch from the `Zones` view to the `Layered Topology` and `Network Topology` views (top right of *Results (#)* table).
   - Which zones interact with each other?
   - For the zones interacting with one another, consider if their interaction make sense. *Should* they be interacting?.
   - Which zones pose more risk than others?
<br/><br/>
5. Return to the `Zones` view and select one with multiple assets to view its zone page.

### REFLECTION
- How can communication patterns between zones help identify potential security concerns?
- How can zones help prioritize investigations and remediation activities?