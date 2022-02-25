---
title: "EntMovement"
slug: "entmovement"
hidden: false
createdAt: "2020-11-10T21:51:06.721Z"
updatedAt: "2021-06-18T01:37:56.227Z"
---
**Movement**
Adds MoveDirection / LookDirection variables for other movement components to use

ID: EntMovement
Requires Components: [Physics](doc:entphysics)
Required By: [Movement AI](doc:entmovementai), [Flying Movement](doc:entflyingmovement), [Animated Humanoid](doc:entanimatedhumanoid), [Walking Movement](doc:entwalkingmovement), [Hover Movement](doc:enthovermovement), [Rotate Transform Towards Look Position](doc:entrotatetransformtowardslookposition)
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
    "0-0": "Move Direction",
    "0-1": "Vector3 Variable",
    "0-2": "Move Direction is the direction in World space to move",
    "1-0": "Look Position",
    "1-1": "Vector3 Variable",
    "1-2": "Look Position is the position in the World to look at"
  },
  "cols": 3,
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
    "0-0": "Look Direction",
    "0-1": "Vector3",
    "0-2": "The direction set by the LookPosition and this Entity's position."
  },
  "cols": 3,
  "rows": 1
}
[/block]