---
title: "EntGrabbablePart"
slug: "entgrabbablepart"
hidden: false
createdAt: "2020-11-10T22:11:20.095Z"
updatedAt: "2021-06-18T01:37:49.220Z"
---
**Grabbable Part**


ID: EntGrabbablePart
Abstract
Required By: [Grabbable Part Grab Sound](doc:entgrabbablepartgrabsound)
Base Type: [Entity Component](doc:componententity)
Base Of: [Pressable Part](doc:entpressablepart), [Movable Part](doc:entmovablepart)

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
    "0-0": "Part Transform",
    "0-1": "Transform Part Variable",
    "0-2": "",
    "1-0": "Not Grabbable",
    "1-1": "Bool Variable",
    "1-2": "",
    "2-0": "Grabbed By",
    "2-1": "Entity Variable",
    "2-2": " - ReadOnly"
  },
  "cols": 3,
  "rows": 3
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