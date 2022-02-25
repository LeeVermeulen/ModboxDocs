---
title: "EntUserBot"
slug: "entuserbot"
hidden: false
createdAt: "2020-11-10T21:51:06.764Z"
updatedAt: "2021-06-18T01:38:07.749Z"
---
**User Bot**
Will add a Bot User that can spawn as a Player Avatar in play mode

ID: EntUserBot
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
    "0-0": "Bot Name",
    "0-1": "Text Variable",
    "0-2": "",
    "1-0": "Spawn At Start",
    "1-1": "Bool Variable",
    "1-2": "Defaults to True",
    "2-0": "Can Spawn",
    "2-1": "Bool Variable",
    "2-2": "Defaults to True",
    "3-0": "Respawn",
    "3-1": "Bool Variable",
    "3-2": "Defaults to True",
    "4-0": "Respawn Time",
    "4-1": "Number Variable",
    "4-2": "Defaults to 3 - s",
    "5-0": "Next Spawn",
    "5-1": "Play Time Variable",
    "5-2": " - ReadOnly"
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
    "0-0": "Set To Random Name",
    "0-1": "",
    "0-2": ""
  },
  "cols": 2,
  "rows": 1
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
    "0-0": "Next Spawn Lapsed()",
    "0-1": "Called when Next Spawn time Lapses"
  },
  "cols": 2,
  "rows": 1
}
[/block]


Attributes:
ModboxMain.MBTypeComponentNoIngameAddingAttribute
ModboxMain.MBTypeComponentEnabledInEditmodeAttribute