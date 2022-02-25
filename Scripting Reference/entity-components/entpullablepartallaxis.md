---
title: "EntPullablePartAllAxis"
slug: "entpullablepartallaxis"
hidden: false
createdAt: "2020-11-10T21:51:07.963Z"
updatedAt: "2021-06-18T01:38:02.025Z"
---
**Pullable Part All Axis**
A part of an Entity that can be grabbed by the player and moved around.

ID: EntPullablePartAllAxis
Base Type: [Pullable Part](doc:entpullablepart)

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
    "0-0": "Current Position",
    "0-1": "Vector3 Variable",
    "0-2": "",
    "1-0": "Current Rotation",
    "1-1": "Vector3 Variable",
    "1-2": "",
    "2-0": "XMotion",
    "2-1": "Enum Variable<Pullable Part Axis Motion>",
    "2-2": "",
    "3-0": "XLimit Range",
    "3-1": "Range Variable",
    "3-2": "degrees",
    "4-0": "YMotion",
    "4-1": "Enum Variable<Pullable Part Axis Motion>",
    "4-2": "",
    "5-0": "YLimit Range",
    "5-1": "Range Variable",
    "5-2": "degrees",
    "6-0": "ZMotion",
    "6-1": "Enum Variable<Pullable Part Axis Motion>",
    "6-2": "",
    "7-0": "ZLimit Range",
    "7-1": "Range Variable",
    "7-2": "degrees",
    "8-0": "Allow Rotation",
    "8-1": "Bool Variable",
    "8-2": "",
    "9-0": "Max Distance",
    "9-1": "Number Variable",
    "9-2": "m",
    "10-0": "Move Back To Start",
    "10-1": "Bool Variable",
    "10-2": "Will move back to start when not grabbed",
    "11-0": "Move Back To Start Speed",
    "11-1": "Number Variable",
    "11-2": "Defaults to 1 - x",
    "12-0": "Part Transform",
    "12-1": "Transform Part Variable",
    "12-2": "",
    "13-0": "Not Grabbable",
    "13-1": "Bool Variable",
    "13-2": "",
    "14-0": "Grabbed By",
    "14-1": "Entity Variable",
    "14-2": " - ReadOnly"
  },
  "cols": 3,
  "rows": 15
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