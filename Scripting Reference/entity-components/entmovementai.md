---
title: "EntMovementAI"
slug: "entmovementai"
hidden: false
createdAt: "2020-11-10T21:51:06.745Z"
updatedAt: "2021-06-18T01:37:55.979Z"
---
**Movement AI**
Controls AI movement. Has a 'Target' variable that sets where AI should look, and a 'MoveGoal' for where to move to

ID: EntMovementAI
Requires Components: [Movement](doc:entmovement)
Required By: [Flying Juke](doc:entflyingjuke), [Movement AI Pathfinding](doc:entmovementaipathfinding)
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
    "1-0": "Target",
    "1-1": "Entity Variable",
    "1-2": "The current Target this AI is looking at",
    "2-0": "Move Goal World Position",
    "2-1": "Vector3 Variable",
    "2-2": "Spot in the world to move to, overridden by MoveGoalEntity",
    "3-0": "Move Goal Entity",
    "3-1": "Entity Variable",
    "3-2": "Entity to Move to, overrides MoveGoalToPosition",
    "4-0": "Move Goal Range",
    "4-1": "Range Variable",
    "4-2": "Range to move into from move goal - m",
    "5-0": "Has Move Goal",
    "5-1": "Bool Variable",
    "5-2": " - ReadOnly",
    "6-0": "Is Within Move Goal Range",
    "6-1": "Bool Variable",
    "6-2": " - ReadOnly",
    "7-0": "Pathfinding Enabled",
    "7-1": "Bool Variable",
    "7-2": "Will add Pathfinding component if needed by Movement controller - Defaults to True"
  },
  "cols": 3,
  "rows": 8
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
    "0-0": "Clear Target And Move Goal",
    "0-1": "",
    "0-2": "",
    "1-0": "Set Target And Move Goal(Entity, Range)",
    "1-1": "",
    "1-2": "Set the Target and make that the Move Goal"
  },
  "cols": 2,
  "rows": 2
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
    "0-0": "Move Goal Current Position",
    "0-1": "Vector3",
    "0-2": "",
    "1-0": "Move Goal Distance",
    "1-1": "Number",
    "1-2": "",
    "2-0": "Target Position",
    "2-1": "Vector3",
    "2-2": "",
    "3-0": "Target Distance",
    "3-1": "Number",
    "3-2": "",
    "4-0": "Target Is Blocked",
    "4-1": "Bool",
    "4-2": "",
    "5-0": "Target Is Blocked By Static",
    "5-1": "Bool",
    "5-2": "",
    "6-0": "Movement Controller",
    "6-1": "Movement AI Controller Interface",
    "6-2": "The current Component controlling the Movement",
    "7-0": "Path Direction",
    "7-1": "Vector3",
    "7-2": "Current direction to Move Goal or next Pathfinding point"
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
    "0-0": "Move Goal First Reached()",
    "0-1": "Called on first reaching a new Move Goal"
  },
  "cols": 2,
  "rows": 1
}
[/block]