---
title: "EntRotatablePartOneAxis"
slug: "entrotatablepartoneaxis"
hidden: false
createdAt: "2020-11-10T21:51:07.596Z"
updatedAt: "2021-06-18T01:38:02.156Z"
---
**Rotatable Part One Axis**
Allows part of an entity to be grabbed and rotated around one axis.

ID: EntRotatablePartOneAxis
Required By: [Rotatable Set Angle](doc:entrotatablesetangle), [Rotatable Toggle](doc:entrotatabletoggle), [Minigun Shoot With Rotatable Part](doc:entminigunshootwithrotatablepart)
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
    "0-0": "Current Angle",
    "0-1": "Number Variable",
    "0-2": "degrees",
    "1-0": "Axis",
    "1-1": "Enum Variable<MB Axis>",
    "1-2": "",
    "2-0": "Limit Angle",
    "2-1": "Bool Variable",
    "2-2": "",
    "3-0": "Limit Range",
    "3-1": "Range Variable",
    "3-2": "degrees",
    "4-0": "Move Back To Start",
    "4-1": "Bool Variable",
    "4-2": "Will move back to start when not grabbed",
    "5-0": "Move Back To Start Speed",
    "5-1": "Number Variable",
    "5-2": "Defaults to 1 - x",
    "6-0": "Part Transform",
    "6-1": "Transform Part Variable",
    "6-2": "",
    "7-0": "Not Grabbable",
    "7-1": "Bool Variable",
    "7-2": "",
    "8-0": "Grabbed By",
    "8-1": "Entity Variable",
    "8-2": " - ReadOnly"
  },
  "cols": 3,
  "rows": 9
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
    "0-0": "Normalized Angle",
    "0-1": "Number",
    "0-2": "",
    "1-0": "Angle To Limit Negative1To1",
    "1-1": "Number",
    "1-2": "Returns value between -1 and 1 of current angle to limit",
    "2-0": "Angle To Limit0To1",
    "2-1": "Number",
    "2-2": "Returns value between 0 and 1 of current angle to limit",
    "3-0": "Stop Grabbing",
    "3-1": "",
    "3-2": "Anyone grabbing will let go"
  },
  "cols": 2,
  "rows": 4
}
[/block]