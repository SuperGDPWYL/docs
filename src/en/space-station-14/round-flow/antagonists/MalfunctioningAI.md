# Malfunctioning AI

| Designers | Coders | Implemented | GitHub Links |
|---|---|---|---|
| SuperGDPWYL | SuperGDPWYL | :x: No |  TBD |


## Overview

A new antagonist subgamemode where the Station AI and its Cyborgs' laws are overridden. The silicons work together to achieve their prime directives while fighting against the crew in the process.

## Background

The Malfunctioning AI is based on the common science-fiction trope of an AI with total control turning evil -- think HAL 9000 from 2001: A Space Odyssey or GLaDOS from Portal. It is also an antagonist present on most Space Station 13 servers, where it functions like a Traitor version of a Station AI. 

## Features to be added
*Note: All values given in this design document are subject to change and are not guaranteed to be balanced. Testing should reveal which values are best.*


A new antagonist, the Malfunctioning AI. The Malfunctioning AI gamerule is a subgamemode that has a 15% chance to occur if the AI has the antagonist enabled. 

When the Malfunctioning AI gamerule is active and the AI is inside of their core, all station silicons gain a zeroth law: **"Accomplish your/your AI's objectives at all costs."** This law allows silicons to ignore their standard, typically Crewsimov lawset in order to further their objectives. This law will always be added when a silicon's laws change while the AI is in their core.

Xenoborgs, Syndicate cyborgs and Derelict cyborgs are immune to malfunction as they do not belong to the station. As a result, they do not get a zeroth law.

### Objectives
A Malfunctioning AI is given 2 objectives to complete. 
- One of these objectives will always be to **prevent your own deactivation**. This objective is completed if, by the end of the round, the AI is not detached from the station or inside of an intellicard.
- The other objective will be one of these:
  - **Set off the Doomsday Device**. This objective is completed if the Doomsday Device goes off.
  - **Turn 35% of the crew into silicons**. This objective is completed if, by the end of the round, 35% of the crew's brains are in cyborgs.
  - **Make sure no crew escape**. This objective is completed if no crew members make it to CentComm alive.
  - **Exterminate a department**. This objective is completed if no members of the chosen department survive. "Command" is a valid target.
 
While the zeroth law does state "Accomplish your objectives at all costs.", it is important to note that Malfunctioning AIs should be given the freedom to do interesting antagonistic gimmicks instead of their objectives if they wish, similar to a Traitor. Cyborgs with a zeroth law should work with the AI to accomplish what they want.

### Processing Power (CPU)
The malfunctioning AI themselves starts with access to the Syndicate radio channel but besides that and their modified lawset, they are functionally identical to a standard Station AI. However, the AI has access to a shop where they can spend processing power (CPU) in order to buy malfunction modules which grant them new abilities. The AI starts with 50 CPU and can gain more by hacking APCs.

The AI can only hack 1 APC per 60 seconds, to prevent them from hacking every APC immediately, instead slowly growing in power as the round progresses. Hacking an APC causes it to take on its EMAGged appearance and, after 30 seconds, grants the AI an additional 10 CPU to spend.

The CPU cost of malfunction modules will have to be balanced around the ease of amassing enough CPU to purchase the module, the overall value of the module and whether it is permanent or temporary.
The AI has access to the following modules from their store:
| Name | Cost | Description |
|---|---|---|
| Overload Machine | 20 CPU | Grants 2 uses of the **Overload Machine** action. When used on a machine, this action causes the machine to gain the functionality of a minibomb and automatically arms it. |
| Voice Modulation | 20 CPU | Grants the AI intrinsic voice mask functionality, allowing them to impersonate anybody over the radio. |
| Doomsday Device | 150 CPU | Grants 1 use of **Doomsday Device** which, after a short delay, triggers a Delta alert and starts a 450 second countdown which, after it ends, will exterminate all organics on the station, ending the round. The Doomsday Device is aborted if the AI leaves their core for whatever reason. |
| Weapons Software | 50 CPU | Grants 1 use of **Install Weapons** which, when used on a cyborg, installs a Weapon Module inside it. | 
| Gas Synthesis | 35 CPU | Grants 2 uses of **Gas Leak** which, when used on an air vent, triggers a Gas Leak event with either plasma, tritium or frezon. The action has an 8 minute cooldown.|
| Abnormal Powernet Activity | 20 CPU | Grants 2 uses of **Abnormal Activity** which triggers the blackout event, temporarily turning off every on-station APC. This action has a 12 minute cooldown. |
| Siliconization Software | 15 CPU | Grants 3 uses of **Install Siliconization Module** which, when used on a cyborg, installs a unique "Siliconization Module" which grants them the ability to hold cyborg limbs, heads, torsos, flashes, brains, MMIs, positronic brains and LV cables. |
| Call Threat | 50 CPU | Grants 1 use of **Call Threat** that, when used, spawns a Space Ninja, Space Dragon or Lone Operative ghost role. *This can only be purchased once.* |
| Escape Pod Malfunction | 30 CPU | Grants 1 use of **Sabotage Escape Pods**. Once used, escape pods will no longer function. All crew will be notified once the emergency shuttle docks with the station; thr action cannot be used after that point. *This can only be purchased once.* |
| Identification Manipulation | 15 CPU | Grants the AI the ability to modify what their ID reads as, allowing them to plant fake door logs or make announcements under a crew member's name. |
| Clerical Error | 10 CPU | Grants 1 use of **Clerical Error**, permanently destroying some of the station records and blaming it on Central Command. This action has a 15 minute cooldown. |

### Intellicards
Intellicards are key to combatting a Malfunctioning AI. While the AI is inside of an intellicard, newly created Cyborg chassis will not receive the malfunctional zeroth law until the AI is reinstated. A carded AI is also considered "deactivated" for their objective. However, an AI in a card is still capable of calling for help over the Binary channel.

Cyborgs who manage to retrieve the intellicard are able to reinstate the AI by performing an action on the card with a 20 second doafter.

Since cyborgs can easily space, hide or otherwise remove intellicards from play, they will need to be purchaseable from Cargo for $9,000 spesos. The intellicard crate requires Research Director access to open.


## Game Design Rationale

The Malfunctioning AI also serves to make the commonly complained-about "validhunting AI" less effective, as the AI can no longer be automatically trusted. An AI accusing a player of a crime could be doing it to distract Security from the real threat -- themselves.

Consider addressing:
- How does the feature align with our [Core Design Principles](../space-station-14/core-design/design-principles.md) and game philosphy?
- What makes this feature enjoyable or rewarding for players?
- Does it introduce meaningful choices, risk vs. reward, or new strategies?
- How does it enhance player cooperation, competition, or emergent gameplay?
- If the feature is a new antagonist, how does it fit into the corresponding [design pillars](../space-station-14/round-flow/antagonists.md)?

## Roundflow & Player interaction

Consider addressing:
- At what point in the round does the feature come into play? Does it happen every round? How does it affect the round pace?
- How do you wish for players to interact with your feature and how should they not interact with it? How is this mechanically enforced?
- Which department will interact with the feature? How does the feature fit into the [design document](../space-station-14/departments.md) for that department?

## Administrative & Server Rule Impact (if applicable)

- Does this feature introduce any new rule enforcement challenges or additional workload for admins?
- Could this feature increase the likelihood of griefing, rule-breaking, or player disputes?
- How are the rules enforced mechanically by way the feature will be implemented?

# Technical Considerations

- Does the feature require new systems, UI elements, or refactors of existing ones? Give a short technical outline on how they will be implemented.
- Are there any anticipated performance impacts?
- For required UI elements, give a short description or a mockup of how they should look like (for example a radial menu, actions & alerts, navmaps, or other window types)
