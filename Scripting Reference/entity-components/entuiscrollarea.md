---
title: "EntUIScrollArea"
slug: "entuiscrollarea"
hidden: false
createdAt: "2020-11-10T21:51:06.952Z"
updatedAt: "2021-06-18T01:38:07.699Z"
---
**UI Scroll Area**
Allows scrolling child UI entities

ID: EntUIScrollArea
Requires Components: [UI Transform](doc:entuitransform)
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
    "0-0": "Scroll Axis",
    "0-1": "Enum Variable<Scroll Axis>",
    "0-2": "",
    "1-0": "Scroll Sensitivity",
    "1-1": "Number Variable",
    "1-2": "Defaults to 10",
    "2-0": "Use Inertia",
    "2-1": "Bool Variable",
    "2-2": "If true, the scroll area will continue moving in the direction it was scrolled.",
    "3-0": "Deceleration",
    "3-1": "Number Variable",
    "3-2": "How fast the scroll area comes to a stop when using Inertia. - Defaults to 0.135",
    "4-0": "Movement Type",
    "4-1": "Enum Variable<Movement Type>",
    "4-2": "Changes how scroll movement is handled. Clamped prevents scrolling past items, Unrestricted allows infinite scrolling, and Elastic allows a little bit of scrolling past items but will bounce back to them"
  },
  "cols": 3,
  "rows": 5
}
[/block]


Attributes:
ModboxMain.MBTypeComponentNoIngameAddingAttribute