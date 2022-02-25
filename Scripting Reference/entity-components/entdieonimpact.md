---
title: "EntDieOnImpact"
slug: "entdieonimpact"
hidden: false
createdAt: "2020-11-10T22:11:20.124Z"
updatedAt: "2021-06-18T01:37:37.949Z"
---
**Die On Impact**
Will die on impact above a min velocity

ID: EntDieOnImpact
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
    "0-0": "Min Velocity",
    "0-1": "Number Variable",
    "0-2": "m/s",
    "1-0": "Only Under Part",
    "1-1": "Transform Part Variable",
    "1-2": "Only if collided under this part"
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
    "0-0": "Should Die On Collision(Collision Info arg1)",
    "0-1": "Bool",
    "0-2": ""
  },
  "cols": 3,
  "rows": 1
}
[/block]