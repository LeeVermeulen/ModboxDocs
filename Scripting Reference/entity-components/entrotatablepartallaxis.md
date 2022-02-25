---
title: "EntRotatablePartAllAxis"
slug: "entrotatablepartallaxis"
hidden: false
createdAt: "2020-11-10T21:51:06.670Z"
updatedAt: "2021-06-18T01:38:02.392Z"
---
**Rotatable Part All Axis**
Allows part of an entity to be grabbed and rotated around every axis.

ID: EntRotatablePartAllAxis
Required By: [Rotatable Set All Angles](doc:entrotatablesetallangles)
Base Type: [Rotatable Part](doc:entrotatablepart)

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
    "0-0": "Current Rotation",
    "0-1": "Vector3 Variable",
    "0-2": "",
    "1-0": "XMotion",
    "1-1": "Enum Variable<Rotable Part Axis Motion>",
    "1-2": "",
    "2-0": "XLimit Range",
    "2-1": "Range Variable",
    "2-2": "degrees",
    "3-0": "YMotion",
    "3-1": "Enum Variable<Rotable Part Axis Motion>",
    "3-2": "",
    "4-0": "YLimit Range",
    "4-1": "Range Variable",
    "4-2": "degrees",
    "5-0": "ZMotion",
    "5-1": "Enum Variable<Rotable Part Axis Motion>",
    "5-2": "",
    "6-0": "ZLimit Range",
    "6-1": "Range Variable",
    "6-2": "degrees",
    "7-0": "Move Back To Start",
    "7-1": "Bool Variable",
    "7-2": "Will move back to start when not grabbed",
    "8-0": "Move Back To Start Speed",
    "8-1": "Number Variable",
    "8-2": "Defaults to 1 - x",
    "9-0": "Part Transform",
    "9-1": "Transform Part Variable",
    "9-2": "",
    "10-0": "Not Grabbable",
    "10-1": "Bool Variable",
    "10-2": "",
    "11-0": "Grabbed By",
    "11-1": "Entity Variable",
    "11-2": " - ReadOnly"
  },
  "cols": 3,
  "rows": 12
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
    "0-0": "Rotation Normalized",
    "0-1": "Vector3",
    "0-2": "Returns rotation as between -180 to 180",
    "1-0": "Angle To Limit Negative1To1",
    "1-1": "Vector3",
    "1-2": "Returns value between -1 and 1 of current angle to limit",
    "2-0": "Angle To Limit0To1",
    "2-1": "Vector3",
    "2-2": "Returns value between 0 and 1 of current angle to limit",
    "3-0": "Stop Grabbing",
    "3-1": "",
    "3-2": "Anyone grabbing will let go"
  },
  "cols": 2,
  "rows": 4
}
[/block]