---
title: "EntEffectRepeat"
slug: "enteffectrepeat"
hidden: false
createdAt: "2020-11-10T22:11:20.119Z"
updatedAt: "2021-06-18T01:37:37.681Z"
---
**Effect Repeat**
Repeat a Effect every # seconds

ID: EntEffectRepeat
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
    "0-0": "Enabled",
    "0-1": "Bool Variable",
    "0-2": "",
    "1-0": "Effect",
    "1-1": "Effect Variable",
    "1-2": "",
    "2-0": "Scale Effects",
    "2-1": "Bool Variable",
    "2-2": "If true the effect will scale to match the transform that the effect is on.",
    "3-0": "On Transform Part",
    "3-1": "Transform Part Variable",
    "3-2": "The transform part that the effect is placed on.",
    "4-0": "Next Effect",
    "4-1": "Play Time Variable",
    "4-2": " - ReadOnly",
    "5-0": "Next Effect Time",
    "5-1": "Number Variable",
    "5-2": "Defaults to 1 - s",
    "6-0": "Random Time",
    "6-1": "Number Variable",
    "6-2": "Add a random variation to next effect time - s"
  },
  "cols": 3,
  "rows": 7
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
    "0-0": "Next Effect Lapsed()",
    "0-1": "Called when Next Effect time Lapses"
  },
  "cols": 2,
  "rows": 1
}
[/block]