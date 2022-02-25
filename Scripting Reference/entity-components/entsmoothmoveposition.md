---
title: "EntSmoothMovePosition"
slug: "entsmoothmoveposition"
hidden: false
createdAt: "2020-11-10T21:51:06.691Z"
updatedAt: "2021-06-18T01:38:02.018Z"
---
**Smooth Move Position**
Directly moves a Entity with MovePosition over time

ID: EntSmoothMovePosition
Required By: [Smooth Move Position Rotate Towards](doc:entsmoothmovepositionrotatetowards)
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
    "0-0": "Moving Enabled",
    "0-1": "Bool Variable",
    "0-2": "Defaults to True",
    "1-0": "Move Type",
    "1-1": "Enum Variable<Smooth Move Type>",
    "1-2": "",
    "2-0": "Move To Entity",
    "2-1": "Entity Component Variable<Transform>",
    "2-2": "The entity transform that this entity will move towards. Overrides Move To Position.",
    "3-0": "Move To Position",
    "3-1": "Vector3 Variable",
    "3-2": "",
    "4-0": "Linear Speed",
    "4-1": "Number Variable",
    "4-2": "m/s",
    "5-0": "Lerp Speed",
    "5-1": "Number Variable",
    "5-2": "x"
  },
  "cols": 3,
  "rows": 6
}
[/block]