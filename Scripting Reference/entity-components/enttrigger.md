---
title: "EntTrigger"
slug: "enttrigger"
hidden: false
createdAt: "2020-11-10T21:51:06.677Z"
updatedAt: "2021-06-18T01:38:07.788Z"
---
**Trigger**
Adds a 'TriggerDown' bool that can be triggered by User Input / AI, that is then used by other components

ID: EntTrigger
Required By: [Gun Charge With Trigger](doc:entgunchargewithtrigger), [Gun Shoot On Releasing Pullable Part](doc:entgunshootonreleasingpullablepart), [Gun Shoot On Trigger](doc:entgunshootontrigger), [Minigun Shoot With Rotatable Part](doc:entminigunshootwithrotatablepart), [Toy Shield](doc:enttoyshield)
Base Type: [Entity Component](doc:componententity)

[block:api-header]
{
  "title": "Values"
}
[/block]

[block:parameters]
{
  "data": {
    "h-0": "Name",
    "h-1": "Type",
    "h-2": "Description",
    "0-0": "Trigger Down",
    "0-1": "Bool Variable",
    "0-2": "Used by other components to Trigger"
  },
  "cols": 3,
  "rows": 1
}
[/block]

[block:api-header]
{
  "title": "Events"
}
[/block]

[block:parameters]
{
  "data": {
    "h-0": "Name",
    "h-1": "Description",
    "0-0": "Trigger Down New()",
    "0-1": "Ran on TriggerDown set to True"
  },
  "cols": 2,
  "rows": 1
}
[/block]