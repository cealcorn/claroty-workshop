---
title: "Investigation"
description: ""
---

The investigation section of Claroty provides a series of pages with data information, such as captured process values and network sessions from assets. These pages, on their own, proivde raw data that can be used to aid in understanding what may have happened to or between assets.

---
## TASK 1: Investigating Process Values
* Navigate to `Investigation` > `Process Values`.
<br/><br/>
* A *process value* is an operational value that an industrial device is monitoring or controlling. 
    * For example, temperature, pressure, on/off state, etc.
    * If you need to answer "What changed?", then investigating process values may be the appropriate next step.
<br/><br/>
* Perhaps recently, the **Chemical_plant** asset had unexpectedly started the **MIX_START** procedure and we need to find out why.
<br/><br/>
* Filter **Access Types** by **Write**.
<br/><br/>
* Search for the process value with the *Target Asset* **Chemical_plant**

![Process value information](../../../assets/ClarotyCTD-Menu-Investigation-ProcessValue.png)

* Open that tag's details and review the information given
    * How many writes were observed for that tag?
    * Which asset issued the commands?
    * What protocol carried the commands?
    * Does this evidence prove that the writes were unauthorized? Why or why not?
    * What evidence should be collected next?
<br/><br/>
* In **Source Assets**, select the listed asset to procede to its page, then switch to the **Comunication** tab.
<br/><br/>
* Under **Baselines**, filter by *Protocol: CIP* and *Access Type: Write* and review the results:
    * Does it appear that it is normal behavior for this asset to issue write commands to *Chemical_plant*?
<br/><br/>
* What other assets has this asset written to, if any?

### TASK 1 REFLECTION

* In a real environment, what would your next step be after discovering the source of the write change?
* What would make a *MIX_START* command suspiscious? 

---

## TASK 2: Investigating Network Sessions
* Navigate to `Investigations` > `Network Sessions`.
<br/><br/>
* A *network session* is a recorded communication between a source asset and a destination asset.
    * Session data can help determine which assets communicate, which services they use, how much traffic they generate, and whether communication problems are occurring.
    * This information can also inform firewall and network-segmentation decisions.
<br/><br/>
* In the results list, sort **Retransmissions** in descending order.
    * Are there any network sessions with a significant amount of retransmissions, especially when compared to packets sent?
    * What kind of situation(s) may cause retransmissions, and what may a high retransmission rate indicate?
<br/><br/>
* *Source* and *Destination Asset* tells us between which two assets the communication is retransmitting. 
    * What is the source asset?
    * What is the destination asset?
<br/><br/>
* Click on the **Destination Asset** to go to its page and determine:
    * What type of asset is it
    * What is its criticality and risk level?
    * What protocol or service is associated with the destination port?
<br/><br/>
* Open the **Communication** tab and review the asset's communication activity.
    * Does the destination communicate with multiple source assets?
    * Do multiple sources experience high retransmission rates when communicating with it?
    * Is the behavior isolated to one source, or does it appear across a shared communication path?
    * Does the communication appear to be part of the asset's normal baseline?
<br/><br/>
* Return to **Network Sessions** and filter by the destination asset.
    * Is the high transmission found in other communications?

### TASK 2 REFLECTION
* How might a high retransmission rate affect a real environment?
* What would be your next steps if you determine this is an isolated issue between two assets? What if it is an issue between multiple different asset communications?