---
title: "EntPhysics"
slug: "entphysics"
hidden: false
createdAt: "2020-11-10T21:51:06.939Z"
updatedAt: "2021-06-25T17:11:05.050Z"
---
**Physics**
Creates or joins a PhysicsBody on play mode

ID: EntPhysics
Required By: [Movement](doc:entmovement), [Set Body Mass](doc:entsetbodymass), [Set Center Of Mass](doc:entsetcenterofmass), [Set Mass](doc:entsetmass)
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
    "0-0": "Material Break",
    "0-1": "Bool Variable",
    "0-2": "Set if it should break based on it's physics material settings (Break On Damage / Break on Impact)",
    "1-0": "Physics Material",
    "1-1": "Physics Material Variable",
    "1-2": "",
    "2-0": "Physics Sound",
    "2-1": "Physics Sound Type Variable",
    "2-2": "Sounds for collision - default set by PhysicsMaterial"
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
    "0-0": "Set Velocity(Vector3 newVelocity)",
    "0-1": "",
    "1-0": "Set Angular Velocity(Vector3 newVelocity)",
    "1-1": "",
    "2-0": "Add Force(Vector3 force, Force Mode mode, Bool relativeToSelf)",
    "2-1": "",
    "3-0": "Add Force At Position(Vector3 force, Vector3 position, Force Mode mode)",
    "3-1": "",
    "4-0": "Add Torque(Vector3 force, Force Mode mode, Bool relativeToSelf)",
    "4-1": ""
  },
  "cols": 2,
  "rows": 5
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
    "0-0": "Mass",
    "0-1": "Number",
    "0-2": "Returns mass based on volume / physics material",
    "1-0": "Center Of Mass",
    "1-1": "Vector3",
    "1-2": "",
    "2-0": "Physics Body",
    "2-1": "PhysicsBody",
    "2-2": ""
  },
  "cols": 3,
  "rows": 3
}
[/block]