---
title: "EntHoverMovement"
slug: "enthovermovement"
hidden: false
createdAt: "2020-11-10T21:51:07.042Z"
updatedAt: "2021-06-18T01:37:49.581Z"
---
**Hover Movement**
Allows an entity to move by hovering along the ground.

ID: EntHoverMovement
Requires Components: [Movement](doc:entmovement)
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
    "1-0": "Hover Only On Movement",
    "1-1": "Bool Variable",
    "1-2": "",
    "2-0": "Height From Ground",
    "2-1": "Number Variable",
    "2-2": "m",
    "3-0": "Max Speed",
    "3-1": "Number Variable",
    "3-2": "m/s",
    "4-0": "Move Speed",
    "4-1": "Number Variable",
    "4-2": "m/s",
    "5-0": "Air Drag",
    "5-1": "Number Variable",
    "5-2": "x",
    "6-0": "Hover Force",
    "6-1": "Number Variable",
    "6-2": "Force applied to Hover above ground - force applied based on height above ground - Defaults to 30 - x",
    "7-0": "Hover Damping",
    "7-1": "Number Variable",
    "7-2": "Defaults to 2 - x",
    "8-0": "Ground Check Radius",
    "8-1": "Number Variable",
    "8-2": "m",
    "9-0": "Set Orientation",
    "9-1": "Enum Variable<Movement Set Orientation>",
    "9-2": "",
    "10-0": "On Ground",
    "10-1": "Bool Variable",
    "10-2": "True if currently hovering on a ground -  - ReadOnly",
    "11-0": "Turn Speed",
    "11-1": "Number Variable",
    "11-2": "Defaults to 1 - x",
    "12-0": "Turn Pitch",
    "12-1": "Bool Variable",
    "12-2": ""
  },
  "cols": 3,
  "rows": 13
}
[/block]