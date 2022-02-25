---
title: "EntDetectorAreaDamage"
slug: "entdetectorareadamage"
hidden: false
createdAt: "2020-11-10T22:11:20.158Z"
updatedAt: "2021-06-18T01:37:37.832Z"
---
**Detector Area Damage**
Do damage to Entities inside the Detector Area

ID: EntDetectorAreaDamage
Requires Components: [Detector Area](doc:entdetectorarea)
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
    "0-0": "Damage Amount",
    "0-1": "Number Variable",
    "0-2": "Defaults to 10 - hp",
    "1-0": "Keep Damaging",
    "1-1": "Bool Variable",
    "1-2": "Will keep damaging every second",
    "2-0": "Time Between Damage",
    "2-1": "Number Variable",
    "2-2": "Defaults to 1 - s",
    "3-0": "Next Damage",
    "3-1": "Play Time Variable",
    "3-2": " - ReadOnly"
  },
  "cols": 3,
  "rows": 4
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
    "0-0": "Next Damage Lapsed()",
    "0-1": "Called when Next Damage time Lapses"
  },
  "cols": 2,
  "rows": 1
}
[/block]