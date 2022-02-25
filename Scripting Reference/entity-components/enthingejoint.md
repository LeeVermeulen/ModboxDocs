---
title: "EntHingeJoint"
slug: "enthingejoint"
hidden: false
createdAt: "2020-11-10T21:59:49.777Z"
updatedAt: "2021-06-18T01:37:49.558Z"
---
**Hinge Joint**
Connects two transforms togther with one axis of rotation.

ID: EntHingeJoint
Required By: [Hinge Joint Motor](doc:enthingejointmotor)
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
    "1-2": "The part that the hinge will rotate around. Will default to this Entity if left blank.",
    "2-0": "Joint Axis",
    "2-1": "Enum Variable<MB Axis>",
    "2-2": "",
    "3-0": "Has Joint Limit",
    "3-1": "Bool Variable",
    "3-2": "Limit the angle this joint can rotate",
    "4-0": "Collide With Connected",
    "4-1": "Bool Variable",
    "4-2": "",
    "5-0": "Max Angle",
    "5-1": "Number Variable",
    "5-2": "degrees",
    "6-0": "Min Angle",
    "6-1": "Number Variable",
    "6-2": "degrees"
  },
  "cols": 3,
  "rows": 7
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
    "0-0": "Angle",
    "0-1": "Number",
    "0-2": "",
    "1-0": "Velocity",
    "1-1": "Number",
    "1-2": ""
  },
  "cols": 3,
  "rows": 2
}
[/block]