# Malfunctioning AI

| Designers | Coders | Implemented | GitHub Links |
|---|---|---|---|
| SuperGDPWYL | SuperGDPWYL | :x: No |  TBD |


## Overview

A new antagonist subgamemode where the Station AI and its Cyborgs' laws are overridden. The silicons work together to achieve their prime directives while fighting against the crew in the process.

## Background

The Malfunctioning AI is based on the common acience-fiction trope of an AI with total control turning evil -- think HAL 9000 from 2001: A Space Odyssey or GLaDOS from Portal. It is also an antagonist present on most Space Station 13 servers, where it functions like a Traitor version of a Station AI. 

The Malfunctioning AI also serves to make the commonly complained-about "validhunting AI" less effective, as the AI can no longer be automatically trusted. An AI accusing a player of a crime could be doing it to distract Security from the real threat -- themselves.

## Features to be added
A new antagonist, the Malfunctioning AI. The Malfunctioning AI gamerule is a subgamemode that has a 15% chance to occur if the AI has the antagonist enabled. 

When the Malfunctioning AI gamerule is active, all station silicons gain a zeroth law: **"Accomplish your/your AI's objectives at all costs."** This law allows silicons to ignore their standard, typically Crewsimov lawset in order to further their objectives. This law will always be added when a silicon's laws change until the AI is defeated.

### Objectives
A Malfunctioning AI is given 3 objectives to complete. 
- One of these objectives will always be to **"Prevent your own deactivation."** This objective is completed if, by the end of the round, the AI is not detached from the station or inside of an intellicard. 

### Processing Power (CPU)
The malfunctioning AI themselves starts with access to the Syndicate radio channel but besides that and their modified lawset, they are functionally identical to a standard Station AI. However, the AI has access to a shop where they can spend processing power (CPU) in order to buy malfunction modules which grant them new abilities. The AI starts with 50 CPU and can gain more by hacking APCs.

The AI can only hack 1 APC per 60 seconds, to prevent them from hacking every APC immediately, instead slowly growing in power as the round progresses. Hacking an APC causes it to take on its EMAGged appearance and grants the AI an additional 10 CPU to spend.

The AI has access to the following modules from their store:
| Name | Cost | Description |
|---|---|---|
| Overload Machine | 20 CPU | Grants 2 uses of the **Overload Machine** action. When used on a machine, this action causes the machine to gain the functionality of a minibomb and automatically arms it. |


Give a description of what game mechanics you would like to add or change. This should be a general overview, with enough details on critical design points that someone can directly implement the feature from this design document. Exact numbers for game balance however are not necessary, as these can be adjusted later either during development or after it has been implemented, but mention *what* will have to be balanced and what needs to be considered when doing so.

## Game Design Rationale

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
