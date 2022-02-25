---
title: "EntTransform"
slug: "enttransform"
hidden: false
createdAt: "2020-11-10T21:51:10.065Z"
updatedAt: "2021-06-25T17:17:04.284Z"
---
**Transform**
Stores 3d position and connection data for entities

ID: EntTransform
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
    "0-0": "Parent",
    "0-1": "Entity Variable",
    "0-2": "",
    "1-0": "Connect To Children",
    "1-1": "Bool Variable",
    "1-2": "Connect children physics bodies together",
    "2-0": "Connect To Parent",
    "2-1": "Bool Variable",
    "2-2": "Connect parent physics body to this ent",
    "3-0": "Start Position",
    "3-1": "Vector3 Variable",
    "3-2": "",
    "4-0": "Start Rotation",
    "4-1": "Vector3 Variable",
    "4-2": "",
    "5-0": "Scale",
    "5-1": "Vector3 Variable",
    "5-2": "",
    "6-0": "Connected To",
    "6-1": "Entity Variable List",
    "6-2": "Entities this Entity is connected to -  - ReadOnly",
    "7-0": "In Ground",
    "7-1": "Bool Variable",
    "7-2": "",
    "8-0": "Static",
    "8-1": "Bool Variable",
    "8-2": "Will set PhysicsBody to Kinematic (not movable)",
    "9-0": "Auto Connect",
    "9-1": "Bool Variable",
    "9-2": "Autoconnect to other entities in edit mode",
    "10-0": "Held By",
    "10-1": "Entity Component Variable<Holder Base>",
    "10-2": "Current Holder entity holding this entity -  - ReadOnly"
  },
  "cols": 3,
  "rows": 11
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
    "0-0": "Move Body Position(Vector3 moveTo)",
    "0-1": "Move Entity to a world position, will move entire physics body if connected to others",
    "1-0": "Move Body Rotation(Vector3 angle)",
    "1-1": "Move Entity to a world rotation, will move entire physics body if connected to others",
    "2-0": "Move Transform Position(Vector3 moveTo)",
    "2-1": "Move just this Entity's transform to a world position. Will move Body if it just has transform",
    "3-0": "Move Transform Rotation(Vector3 rotateTo)",
    "3-1": "Move just this Entity's transform to a world rotation. Will move Body if it just has transform",
    "4-0": "Disconnect()",
    "4-1": "Disconnect from current physics body",
    "5-0": "Connect To(Entity otherEnt)",
    "5-1": "Connect to another physics body during playmode",
    "6-0": "Set Parent(Entity newParent, Bool keepPosition)",
    "6-1": "Set new Parent but keep World position"
  },
  "cols": 2,
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
    "0-0": "Transform Parts",
    "0-1": "Transform Part List",
    "0-2": "All Transform Parts under this Entity",
    "1-0": "Position",
    "1-1": "Vector3",
    "1-2": "Returns current position in the world",
    "2-0": "Rotation",
    "2-1": "Vector3",
    "2-2": "Returns current rotation in the world",
    "3-0": "Transform Part",
    "3-1": "Transform Part",
    "3-2": "The main Transform",
    "4-0": "Transform Part Eye",
    "4-1": "Transform Part",
    "4-2": "The Eye transform set by Components on the Entity",
    "5-0": "Transform Part Center",
    "5-1": "Transform Part",
    "5-2": "The Center transform set by Components on the Entity",
    "6-0": "Physics Body",
    "6-1": "PhysicsBody",
    "6-2": "Play mode PhysicsBody",
    "7-0": "In Water",
    "7-1": "Bool",
    "7-2": "",
    "8-0": "Can See Entity",
    "8-1": "Bool",
    "8-2": "Checks if any colliders are blocking this Entity from seeing another one. Will use the 'Eye' transform if set",
    "9-0": "Children",
    "9-1": "Entity List",
    "9-2": "",
    "10-0": "Children In Asset",
    "10-1": "Entity List",
    "10-2": "Entity Children that are in the Entity's asset"
  },
  "cols": 3,
  "rows": 11
}
[/block]


Attributes:
ModboxMain.MBTypeComponentNoIngameAddingAttribute