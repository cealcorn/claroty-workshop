---
title: "Threat Detection: Overview"
description: "✅"
---
## SCENARIO / CONTEXT
- Gain a high-level understanding of current threat activity within the environment
- Determine where to begin investigating suspicious activity
- Understand the difference between alerts, events, and stories
- Understand the purpose of the various rules

---
## TASK 1: Overview
* Navigate to `Threat Detection` > `Overview`.
<br/><br/>
* Using the information available on the page, determine:
   - The total number of *Open Alerts*
   - The total number of *Events*
   - The number of *Open Stories*

## TASK 1 REFLECTION
* What
* Why

---
## TASK 2: Events vs Alerts vs Stories

Events represent activities that occurred on the network, and not every event is malicious.
Alerts are generated when events meet specific criteria or detection logic.
Stories are collections of related alerts (and events).

### TASK 2 REFLECTION
* what
* why

---
## TASK 3: Rules
* CTD uses several different rule types to determine when alerts should be generated. These rules can be reviewed under `Threat Detection` > `Rules` > `...`.

| title | description |
|:-|:-|
| Zone Rules | Define which zones are expected to communicate with other zones. Zone rules should be validated. |
| Baseline Rules | Define normal network behavior such as typical communication frequency/patterns, timing, protocols, and packet characteristics. |
| Network Signatures | Detect known suspicious or malicious network activity, similar to network-based intrusion detection signatures. They are used to identitfy behaviors such as scanning, explotataion attempts, or other known attack techniques. |
| YARA Rules | Detect known malicious files or file characteristics using pattern mathcing against known indicators to identity malware and suspicious payloads. |
| Auto Resolve | Automatically closes alerters that meet predefined conditions, which helps to reduce alert fatique by resolving expected or previously reviewed activity. |

<!-- - **Zone Rules**
    - Define which zones are expected to communicate with one another.
    - Should be validated.
- **Baseline Rules**
    - Define normal network behavior such as typical communication frequency, timing, protocols, and packet characteristics.
- **Network Signatures**
    - Detect known suspicious or malicious network activity, similar to network-based intrusion detection signatures.
    - Used to identify behaviors such as scanning, exploitation attempts, or other known attack techniques.
- **YARA Rules**
    - Detect known malicious files or file characteristics using pattern matching against known indicators to identify malware and suspicious payloads.
- **Auto Resolve**
    - Automatically closes alerts that meet predefined conditions, which helps reduce alert fatigue by resolving expected or previously reviewed activity. -->

### TASK 3 REFLECTION
* what
* who
<!-- ---
## REFLECTION
- What information can be learned from the Overview page alone?
- If you were beginning an investigation, where would you go next and why?
- What assets or zones appear to require additional attention?
- How does the Threat Detection Overview differ from the Risks & Vulnerabilities Overview? -->