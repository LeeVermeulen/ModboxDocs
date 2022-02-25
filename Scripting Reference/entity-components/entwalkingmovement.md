---
title: "EntWalkingMovement"
slug: "entwalkingmovement"
hidden: false
createdAt: "2020-11-10T21:51:06.698Z"
updatedAt: "2021-06-18T01:38:07.798Z"
---
**Walking Movement**
Movement component for entities that walk on the ground.

ID: EntWalkingMovement
Requires Components: [Movement](doc:entmovement), [Jump](doc:entjump)
Required By: [Animated Humanoid](doc:entanimatedhumanoid)
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
    "0-0": "Enabled",
    "0-1": "Bool Variable",
    "0-2": "Defaults to True",
    "1-0": "Run Speed",
    "1-1": "Number Variable",
    "1-2": "Maximum speed for running - m/s",
    "2-0": "Run",
    "2-1": "Bool Variable",
    "2-2": "",
    "3-0": "Physics Move Mode",
    "3-1": "Bool Variable",
    "3-2": "Move by physics rather than Animation (if this is a Humanoid/Animated)",
    "4-0": "Turn To Look Position",
    "4-1": "Bool Variable",
    "4-2": "Set to turn body towards look position (rather than just head)",
    "5-0": "Air Speed",
    "5-1": "Number Variable",
    "5-2": "m/s",
    "6-0": "Add Gravity",
    "6-1": "Number Variable",
    "6-2": "Add additional gravity in air - Defaults to 2 - x",
    "7-0": "Walk Multiply",
    "7-1": "Number Variable",
    "7-2": "Walk speed as a multiple of RunSpeed - Defaults to 0.5 - x",
    "8-0": "Physics Move Control",
    "8-1": "Number Variable",
    "8-2": "How quickly to change to new movement velocity in Physics Move mode - Defaults to 8 - x",
    "9-0": "Zero G Move Control",
    "9-1": "Number Variable",
    "9-2": "How quickly to change to new movement while in Zero G movement / Flying - Defaults to 6 - x",
    "10-0": "Fly Mode",
    "10-1": "Bool Variable",
    "10-2": "",
    "11-0": "Jump Speed",
    "11-1": "Number Variable",
    "11-2": "m/s"
  },
  "cols": 3,
  "rows": 12
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
    "0-0": "On Ground",
    "0-1": "Bool",
    "0-2": "",
    "1-0": "On Ground Physics Material",
    "1-1": "Physics Material",
    "1-2": ""
  },
  "cols": 3,
  "rows": 2
}
[/block]