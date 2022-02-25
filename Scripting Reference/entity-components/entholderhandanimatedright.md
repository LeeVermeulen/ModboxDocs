---
title: "EntHolderHandAnimatedRight"
slug: "entholderhandanimatedright"
hidden: false
createdAt: "2020-11-10T21:59:50.467Z"
updatedAt: "2021-06-18T01:37:49.599Z"
---
**Holder Hand Animated Right**


ID: EntHolderHandAnimatedRight
Requires Components: [Animated Humanoid](doc:entanimatedhumanoid)
Base Type: [Holder Hand Animated](doc:entholderhandanimated)

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
    "0-2": "Will set TriggerDown on held Trigger component, or Trigger animations set by held entities",
    "1-0": "Trigger Down Until Action",
    "1-1": "Bool Variable",
    "1-2": "Will set TriggerDown until the held Entity is used (charged and fire / triggered animation)",
    "2-0": "Aim Held",
    "2-1": "Bool Variable",
    "2-2": "If should set animation to aim - Defaults to True",
    "3-0": "Drop On Death",
    "3-1": "Bool Variable",
    "3-2": "If held entity should drop on death, otherwise will be removed",
    "4-0": "Default Entity",
    "4-1": "Entity Asset Variable",
    "4-2": "Entity asset the holder will create and start with",
    "5-0": "Scale Default Entity",
    "5-1": "Bool Variable",
    "5-2": "",
    "6-0": "Holding",
    "6-1": "Entity Variable",
    "6-2": "Entity held by holder",
    "7-0": "Holder Position",
    "7-1": "Transform Part Variable",
    "7-2": ""
  },
  "cols": 3,
  "rows": 8
}
[/block]

[block:api-header]
{
  "title": "Properties"
}
[/block]

[block:parameters]
{
  "data": {
    "h-0": "Name",
    "h-1": "Type",
    "h-2": "Description",
    "0-0": "Is Left Hand",
    "0-1": "Bool",
    "0-2": ""
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
    "0-0": "Held Gun Fired()",
    "0-1": ""
  },
  "cols": 2,
  "rows": 1
}
[/block]


Attributes:
ModboxMain.MBTypeComponentNoIngameAddingAttribute