---
title: "EntMovablePart"
slug: "entmovablepart"
hidden: false
createdAt: "2020-11-10T21:51:06.892Z"
updatedAt: "2021-06-18T01:37:56.110Z"
---
**Movable Part**
A grabble part that can be moved/rotated

ID: EntMovablePart
Base Type: [Grabbable Part](doc:entgrabbablepart)
Base Of: [Pullable Part](doc:entpullablepart), [Rotatable Part](doc:entrotatablepart)

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
    "0-0": "Move Back To Start",
    "0-1": "Bool Variable",
    "0-2": "Will move back to start when not grabbed",
    "1-0": "Move Back To Start Speed",
    "1-1": "Number Variable",
    "1-2": "Defaults to 1 - x",
    "2-0": "Part Transform",
    "2-1": "Transform Part Variable",
    "2-2": "",
    "3-0": "Not Grabbable",
    "3-1": "Bool Variable",
    "3-2": "",
    "4-0": "Grabbed By",
    "4-1": "Entity Variable",
    "4-2": " - ReadOnly"
  },
  "cols": 3,
  "rows": 5
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


Attributes:
ModboxMain.MBTypeComponentNoIngameAddingAttribute