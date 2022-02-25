---
title: "EntPlayerSpawnSpot"
slug: "entplayerspawnspot"
hidden: false
createdAt: "2020-11-10T21:51:06.837Z"
updatedAt: "2021-06-25T17:11:05.127Z"
---
**Player Spawn Spot**
Used by User's to select a spawn spot

ID: EntPlayerSpawnSpot
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
    "0-0": "Spawn On Ground",
    "0-1": "Bool Variable",
    "0-2": "If true players will spawn on the surface below the spawn point rather than at it's exact position. - Defaults to True",
    "1-0": "Random Spot Inside",
    "1-1": "Bool Variable",
    "1-2": "Will spawn at a random postion inside the SpawnSpot's area",
    "2-0": "Only If Player Set To Team",
    "2-1": "Team Variable",
    "2-2": "Will only allows players set to this Team to spawn here"
  },
  "cols": 3,
  "rows": 3
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
    "0-0": "Get Spawn Position",
    "0-1": "Vector3",
    "0-2": "",
    "1-0": "Get Ground Position",
    "1-1": "Vector3",
    "1-2": ""
  },
  "cols": 3,
  "rows": 2
}
[/block]

[block:api-header]
{
  "title": "Return Value Events"
}
[/block]

[block:parameters]
{
  "data": {
    "h-0": "Name",
    "h-1": "Type",
    "h-2": "Description",
    "0-0": "Can User Use Spot(User arg1)",
    "0-1": "Bool",
    "0-2": "Can set if a User can use this Spawn Spot"
  },
  "cols": 3,
  "rows": 1
}
[/block]


Attributes:
ModboxMain.MBTypeComponentNoIngameAddingAttribute