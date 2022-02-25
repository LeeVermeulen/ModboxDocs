---
title: "EntSpawner"
slug: "entspawner"
hidden: false
createdAt: "2020-11-10T21:51:07.529Z"
updatedAt: "2021-06-18T01:38:02.398Z"
---
**Spawner**
Spawn and launch entities with velocity / spread

ID: EntSpawner
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
    "0-0": "Spawn Effect",
    "0-1": "Effect Variable",
    "0-2": "",
    "1-0": "Spawn Entity Asset",
    "1-1": "Entity Asset Variable",
    "1-2": "",
    "2-0": "Spawning",
    "2-1": "Bool Variable",
    "2-2": "Defaults to True",
    "3-0": "Fire Rate",
    "3-1": "Number Variable",
    "3-2": "Defaults to 1 - s",
    "4-0": "Fire Immediately",
    "4-1": "Bool Variable",
    "4-2": "If true the spawner will spawn an object right away when entering play mode instead of waiting for the fire rate interval.",
    "5-0": "Launch Speed",
    "5-1": "Number Variable",
    "5-2": "Defaults to 5 - m/s",
    "6-0": "Max Amount",
    "6-1": "Int Variable",
    "6-2": "Defaults to 1 - #",
    "7-0": "Spread Type",
    "7-1": "Enum Variable<Spawner Spread Type>",
    "7-2": "",
    "8-0": "Spread",
    "8-1": "Number Variable",
    "8-2": "degrees",
    "9-0": "On Max Amount",
    "9-1": "Enum Variable<Spawn On Max Amount>",
    "9-2": "Defaults to StopSpawning",
    "10-0": "Reuse Entities",
    "10-1": "Bool Variable",
    "10-2": "When 'RemoveOldest' is on the same Entities will be moved to be launched again rather than spawn new entities. - Defaults to True",
    "11-0": "Next Spawn",
    "11-1": "Play Time Variable",
    "11-2": "",
    "12-0": "Spawn Rotation",
    "12-1": "Vector3 Variable",
    "12-2": "",
    "13-0": "Spawned List",
    "13-1": "Entity Variable List",
    "13-2": " - ReadOnly"
  },
  "cols": 3,
  "rows": 14
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
    "0-0": "Spawn()",
    "0-1": "",
    "1-0": "Spawn At Speed(Vector3 velocity)",
    "1-1": ""
  },
  "cols": 2,
  "rows": 2
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
    "0-0": "Entity Spawned(Entity spawned)",
    "0-1": "",
    "1-0": "Next Spawn Lapsed()",
    "1-1": "Called when Next Spawn time Lapses"
  },
  "cols": 2,
  "rows": 2
}
[/block]