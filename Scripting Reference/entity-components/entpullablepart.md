---
title: "EntPullablePart"
slug: "entpullablepart"
hidden: false
createdAt: "2020-11-10T21:51:06.774Z"
updatedAt: "2021-06-18T01:38:02.081Z"
---
**Pullable Part**
A Pullable Part is a grabbable part of a entity that can be grabbed and pulled

ID: EntPullablePart
Required By: [Pullable Part Rotate Towards Start](doc:entpullablepartrotatetowardsstart), [Gun Charge With Pullable Part](doc:entgunchargewithpullablepart), [Gun Shoot On Releasing Pullable Part](doc:entgunshootonreleasingpullablepart), [Toy Face Pulled Direction](doc:enttoyfacepulleddirection)
Base Type: [Movable Part](doc:entmovablepart)
Base Of: [Pullable Part One Axis](doc:entpullablepartoneaxis), [Pullable Part All Axis](doc:entpullablepartallaxis)

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
    "0-0": "Max Distance",
    "0-1": "Number Variable",
    "0-2": "m",
    "1-0": "Move Back To Start",
    "1-1": "Bool Variable",
    "1-2": "Will move back to start when not grabbed",
    "2-0": "Move Back To Start Speed",
    "2-1": "Number Variable",
    "2-2": "Defaults to 1 - x",
    "3-0": "Part Transform",
    "3-1": "Transform Part Variable",
    "3-2": "",
    "4-0": "Not Grabbable",
    "4-1": "Bool Variable",
    "4-2": "",
    "5-0": "Grabbed By",
    "5-1": "Entity Variable",
    "5-2": " - ReadOnly"
  },
  "cols": 3,
  "rows": 6
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
    "0-0": "Stop Grabbing",
    "0-1": "",
    "0-2": "Anyone grabbing will let go"
  },
  "cols": 2,
  "rows": 1
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
    "0-0": "Distance Ratio",
    "0-1": "Number",
    "0-2": "Returns value of current distance to limit (-1 to 1 value)",
    "1-0": "World Distance",
    "1-1": "Number",
    "1-2": ""
  },
  "cols": 3,
  "rows": 2
}
[/block]


Attributes:
ModboxMain.MBTypeComponentNoIngameAddingAttribute