---
title: "EntPullablePartOneAxis"
slug: "entpullablepartoneaxis"
hidden: false
createdAt: "2020-11-10T21:51:06.864Z"
updatedAt: "2021-06-18T01:38:02.047Z"
---
**Pullable Part One Axis**
Allows part of an entity to be moved on one axis.

ID: EntPullablePartOneAxis
Required By: [Pullable Part Toggle](doc:entpullableparttoggle), [Gun Load With Pullable Part](doc:entgunloadwithpullablepart)
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
    "0-0": "Axis",
    "0-1": "Enum Variable<MB Axis>",
    "0-2": "",
    "1-0": "Current Position",
    "1-1": "Number Variable",
    "1-2": "m (local)",
    "2-0": "Limit By Range",
    "2-1": "Bool Variable",
    "2-2": "",
    "3-0": "Limit Range",
    "3-1": "Range Variable",
    "3-2": "m (local)",
    "4-0": "Max Distance",
    "4-1": "Number Variable",
    "4-2": "m",
    "5-0": "Move Back To Start",
    "5-1": "Bool Variable",
    "5-2": "Will move back to start when not grabbed",
    "6-0": "Move Back To Start Speed",
    "6-1": "Number Variable",
    "6-2": "Defaults to 1 - x",
    "7-0": "Part Transform",
    "7-1": "Transform Part Variable",
    "7-2": "",
    "8-0": "Not Grabbable",
    "8-1": "Bool Variable",
    "8-2": "",
    "9-0": "Grabbed By",
    "9-1": "Entity Variable",
    "9-2": " - ReadOnly"
  },
  "cols": 3,
  "rows": 10
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
    "0-0": "Get Max Distance Position",
    "0-1": "Vector3",
    "0-2": "",
    "1-0": "Stop Grabbing",
    "1-1": "",
    "1-2": "Anyone grabbing will let go"
  },
  "cols": 2,
  "rows": 2
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