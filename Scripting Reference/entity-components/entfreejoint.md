---
title: "EntFreeJoint"
slug: "entfreejoint"
hidden: false
createdAt: "2020-11-10T22:11:20.407Z"
updatedAt: "2021-06-18T01:37:38.174Z"
---
**Free Joint**
Joint that can rotate in all / certain angles

ID: EntFreeJoint
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
    "1-2": "Part in this Entity to connect. If left blank it will use the top transform in this entity.",
    "2-0": "Collide With Connected",
    "2-1": "Bool Variable",
    "2-2": "",
    "3-0": "Offset",
    "3-1": "Vector3 Variable",
    "3-2": "",
    "4-0": "XMotion",
    "4-1": "Enum Variable<Configurable Joint Motion>",
    "4-2": "The motion type that influences movement on the X axis. Free alows unrestrained movement on the X axis, Limited alows for movement within the Linear Limit, and Locked prevents all movement on the X axis.",
    "5-0": "YMotion",
    "5-1": "Enum Variable<Configurable Joint Motion>",
    "5-2": "The motion type that influences movement on the Y axis. Free alows unrestrained movement on the Y axis, Limited alows for movement within the Linear Limit, and Locked prevents all movement on the Y axis.",
    "6-0": "ZMotion",
    "6-1": "Enum Variable<Configurable Joint Motion>",
    "6-2": "The motion type that influences movement on the Z axis. Free alows unrestrained movement on the Z axis, Limited alows for movement within the Linear Limit, and Locked prevents all movement on the Z axis.",
    "7-0": "Linear Limit",
    "7-1": "Number Variable",
    "7-2": "The range of movement allowed on Limited axes. This value is used for both positive and negative movement. - m",
    "8-0": "Angular X Motion",
    "8-1": "Enum Variable<Configurable Joint Motion>",
    "8-2": "The motion type that influences rotation along the X axis. - Defaults to Free",
    "9-0": "Low Angular X Limit",
    "9-1": "Number Variable",
    "9-2": "The minimum limit for X axis rotation. Cannot be higher than the High Angular X Limit. - degrees",
    "10-0": "High Angular X Limit",
    "10-1": "Number Variable",
    "10-2": "The maximum limit for X axis rotation. Cannot be lower than the Low Angular X Limit. - degrees",
    "11-0": "Angular Y Motion",
    "11-1": "Enum Variable<Configurable Joint Motion>",
    "11-2": "The motion type that influences rotation along the Y axis. Free alows unrestreained rotation on the X axis, Limited alows for rotation between the High and Low Angular X Limit, and Locked prevents all rotation on the X axis. - Defaults to Free",
    "12-0": "Angular Y Limit",
    "12-1": "Number Variable",
    "12-2": "The range of rotation allowed on the Y axis. This value is used for both positive and negative rotation. - degrees",
    "13-0": "Angular Z Motion",
    "13-1": "Enum Variable<Configurable Joint Motion>",
    "13-2": "The motion type that influences rotation along the Z axis. Free alows unrestreained rotation on the Z axis, Limited alows for rotation within Angular Z Limit, and Locked prevents all rotation on the Z axis. - Defaults to Free",
    "14-0": "Angular Z Limit",
    "14-1": "Number Variable",
    "14-2": "The range of rotation allowed on the Z axis. This value is used for both positive and negative rotation. - degrees"
  },
  "cols": 3,
  "rows": 15
}
[/block]