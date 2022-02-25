---
title: "EntEffectLoop"
slug: "enteffectloop"
hidden: false
createdAt: "2020-11-10T22:11:20.103Z"
updatedAt: "2021-06-18T01:37:37.994Z"
---
**Effect Loop**
Plays a Effect on loop. This only loops the effect visual, to loop the effect sound and physics use Effect Repeat.

ID: EntEffectLoop
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
    "2-0": "Set Effect Scale",
    "2-1": "Bool Variable",
    "2-2": "If true effect will be set to scale to match the transform that the effect is on.",
    "3-0": "Effect Scale",
    "3-1": "Number Variable",
    "3-2": "Defaults to 1 - x",
    "4-0": "Set Effect Space",
    "4-1": "Bool Variable",
    "4-2": "If true can override the effect's simulation space to be World or Local.",
    "5-0": "Effect Space",
    "5-1": "Enum Variable<Effect Space>",
    "5-2": "",
    "6-0": "On Transform Part",
    "6-1": "Transform Part Variable",
    "6-2": "The transform part that the effect is placed on."
  },
  "cols": 3,
  "rows": 7
}
[/block]

[block:api-header]
{
  "title": "Methods"
}
[/block]

[block:parameters]
{
  "data": {
    "h-0": "Name",
    "h-1": "Description",
    "0-0": "Reset Particle()",
    "0-1": "Resets Particle Effect"
  },
  "cols": 2,
  "rows": 1
}
[/block]