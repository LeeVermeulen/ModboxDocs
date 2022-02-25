---
title: "EntDetectorArea"
slug: "entdetectorarea"
hidden: false
createdAt: "2020-11-10T22:11:20.136Z"
updatedAt: "2021-06-18T01:37:37.790Z"
---
**Detector Area**
Detects Entities inside it's bounds

ID: EntDetectorArea
Required By: [Detector Area Damage](doc:entdetectorareadamage)
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
    "0-2": "Defaults to True",
    "1-0": "Filter By Tag",
    "1-1": "Tag On Entity Variable List",
    "1-2": "Only run event if other Entity has all of these tags",
    "2-0": "Filter By Component",
    "2-1": "Entity Component Type Variable List",
    "2-2": "Only run event if other Entity has all of these components",
    "3-0": "Visible In Playmode",
    "3-1": "Bool Variable",
    "3-2": "",
    "4-0": "Shape",
    "4-1": "Enum Variable<Detector Area Shape>",
    "4-2": "",
    "5-0": "Area Scale",
    "5-1": "Vector3 Variable",
    "5-2": "",
    "6-0": "Total Inside",
    "6-1": "Int Variable",
    "6-2": "# -  - ReadOnly"
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
    "0-0": "Inside Entities",
    "0-1": "Entity List",
    "0-2": "",
    "1-0": "Inside Entities All",
    "1-1": "Entity List",
    "1-2": "Uses a Physics cast to check for all Entities inside area including Static",
    "2-0": "Position Inside Detector",
    "2-1": "Bool",
    "2-2": ""
  },
  "cols": 2,
  "rows": 3
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
    "0-0": "Enter(Entity otherEnt)",
    "0-1": "",
    "1-0": "Exit(Entity otherEnt)",
    "1-1": ""
  },
  "cols": 2,
  "rows": 2
}
[/block]