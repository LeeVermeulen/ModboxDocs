---
title: "EntSpringJoint"
slug: "entspringjoint"
hidden: false
createdAt: "2020-11-10T21:51:06.918Z"
updatedAt: "2021-06-18T01:38:02.253Z"
---
**Spring Joint**
Connects two transforms togther with a spring.

ID: EntSpringJoint
Required By: [Spring Joint Line](doc:entspringjointline)
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
    "0-0": "Connected To",
    "0-1": "Transform Part Variable",
    "0-2": "",
    "1-0": "Connected From",
    "1-1": "Transform Part Variable",
    "1-2": "The transform in this entity that will be connected. Will default to the top transform if left blank.",
    "2-0": "Collide With Connected",
    "2-1": "Bool Variable",
    "2-2": "",
    "3-0": "Set Distance At Start",
    "3-1": "Bool Variable",
    "3-2": "",
    "4-0": "Min Distance",
    "4-1": "Number Variable",
    "4-2": "m",
    "5-0": "Max Distance",
    "5-1": "Number Variable",
    "5-2": "m",
    "6-0": "Spring",
    "6-1": "Number Variable",
    "6-2": "kn",
    "7-0": "Damper",
    "7-1": "Number Variable",
    "7-2": "x",
    "8-0": "Break Force",
    "8-1": "Number Variable",
    "8-2": ""
  },
  "cols": 3,
  "rows": 9
}
[/block]


Attributes:
ModboxMain.MBTypeComponentEnabledInEditmodeAttribute