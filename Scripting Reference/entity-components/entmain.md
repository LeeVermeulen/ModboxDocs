---
title: "EntMain"
slug: "entmain"
hidden: false
createdAt: "2020-11-10T21:51:06.702Z"
updatedAt: "2021-06-18T01:37:56.270Z"
---
**Main**
Main Entity Component, storing name and other core data

ID: EntMain
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
    "0-0": "Name",
    "0-1": "Text Variable",
    "0-2": "",
    "1-0": "Entity Disabled",
    "1-1": "Bool Variable",
    "1-2": "",
    "2-0": "MB Prefab",
    "2-1": "Entity Prefab Asset Variable",
    "2-2": "Prefab this Entity is using -  - ReadOnly",
    "3-0": "Tags",
    "3-1": "Text Variable List",
    "3-2": "List of tags added to the Entity",
    "4-0": "Added Components",
    "4-1": "Entity Component Type Variable List",
    "4-2": "List component types that have been added to the Entity -  - ReadOnly",
    "5-0": "Removed Components",
    "5-1": "Entity Component Type Variable List",
    "5-2": "List component types removed from the Entity that were on it's Asset"
  },
  "cols": 3,
  "rows": 6
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
    "0-0": "All Components",
    "0-1": "Entity Component List",
    "0-2": "All Components on the Entity",
    "1-0": "Owned By",
    "1-1": "Client",
    "1-2": "Returns the client that is set as the Entity Owner. Set if this is a User/PlayerAvatar or held by one.",
    "2-0": "Controlled By",
    "2-1": "Client",
    "2-2": "Returns who is 'controlling' this Entity currently. If it has a Owner it will be the owner - or who is moving the physics body",
    "3-0": "Has Tag",
    "3-1": "Bool",
    "3-2": "Returns true if entity has the tag or Asset has tag",
    "4-0": "Remove Component Type",
    "4-1": "",
    "4-2": "",
    "5-0": "Add Component",
    "5-1": "",
    "5-2": "Add a Component Type and it's required components",
    "6-0": "Remove Entity()",
    "6-1": "Removes the entity from the world",
    "7-0": "Turn On Playmode()",
    "7-1": "",
    "8-0": "Die()",
    "8-1": "Kills the entity (break apart / ragdoll)",
    "9-0": "Refresh Values()",
    "9-1": "Runs RefreshValues event which components can use to refresh their values",
    "10-0": "Reset All Values()",
    "10-1": "Resets the values all components to their prefab or default value",
    "11-0": "Reset Values On(MB Type Entity Component component)",
    "11-1": "Resets the values on a given component type to their prefab or default value",
    "12-0": "Play Audio(Audio Clip clip)",
    "12-1": "Play Audio on Entity. Sound will follow Entity will stop last audio played"
  },
  "cols": 2,
  "rows": 13
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
    "0-0": "Asset",
    "0-1": "Entity Asset",
    "0-2": "Asset this Entity was created from",
    "1-0": "Asset Tags",
    "1-1": "Text List",
    "1-2": "Tags on the Asset this Entity was created from",
    "2-0": "In Play Mode",
    "2-1": "Bool",
    "2-2": "",
    "3-0": "Ent ID",
    "3-1": "Whole Number",
    "3-2": "",
    "4-0": "Is Local Only Entity",
    "4-1": "Bool",
    "4-2": "",
    "5-0": "Is Disabled In Hierarchy",
    "5-1": "Bool",
    "5-2": "Entity is Disabled or a parent is Disabled",
    "6-0": "Is Dead",
    "6-1": "Bool",
    "6-2": "",
    "7-0": "Using Prefabs",
    "7-1": "MB Prefab Instance List",
    "7-2": ""
  },
  "cols": 3,
  "rows": 8
}
[/block]

[block:api-header]
{
  "title": "Events"
}
[/block]

[block:parameters]
{
  "data": {
    "h-0": "Name",
    "h-1": "Description",
    "0-0": "Awake()",
    "0-1": "Ran after the Entity is created before starting play mode",
    "1-0": "Start()",
    "1-1": "Ran when the Entity starts in play mode",
    "2-0": "Update()",
    "2-1": "Ran between 5-10 times a second",
    "3-0": "Update Second()",
    "3-1": "Ran at near every second",
    "4-0": "Enabled In Hierarchy()",
    "4-1": "Ran when the Entity is enabled",
    "5-0": "Disabled In Hierarchy()",
    "5-1": "Ran when the Entity is disabled",
    "6-0": "Refreshed Values()",
    "6-1": "Ran by components to clear values / refresh state. Also ran after components are added/removed",
    "7-0": "Removed()",
    "7-1": "Ran when Entity is removed",
    "8-0": "On Death()",
    "8-1": "Ran when Entity dies"
  },
  "cols": 2,
  "rows": 9
}
[/block]


Attributes:
ModboxMain.MBTypeComponentNoIngameAddingAttribute