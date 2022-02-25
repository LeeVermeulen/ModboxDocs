---
title: "EntRespawn"
slug: "entrespawn"
hidden: false
createdAt: "2020-11-10T21:51:06.980Z"
updatedAt: "2021-06-18T01:38:02.102Z"
---
**Respawn**
Respawn a entity after its dead. Will respawn Entity as it was when it entered play mode

ID: EntRespawn
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
    "0-0": "Respawn After Death",
    "0-1": "Bool Variable",
    "0-2": "Defaults to True",
    "1-0": "Respawn After Death Time",
    "1-1": "Number Variable",
    "1-2": "How many seconds it will take for the entity to respawn after it has been removed. - Defaults to 1 - s"
  },
  "cols": 3,
  "rows": 2
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
    "0-0": "Instant Respawn()",
    "0-1": "Dies and respawns the entity instantly"
  },
  "cols": 2,
  "rows": 1
}
[/block]