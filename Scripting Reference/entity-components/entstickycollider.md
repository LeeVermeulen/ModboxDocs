---
title: "EntStickyCollider"
slug: "entstickycollider"
hidden: false
createdAt: "2020-11-10T21:51:06.775Z"
updatedAt: "2021-06-18T01:38:02.312Z"
---
**Sticky Collider**
Causes the entity to stick to other objects by creating a joint on collision.

ID: EntStickyCollider
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
    "0-0": "Break On Force",
    "0-1": "Bool Variable",
    "0-2": "Defaults to True",
    "1-0": "Break Force",
    "1-1": "Number Variable",
    "1-2": "The force required to 'un-stick' the entity. - kn",
    "2-0": "Minimum Speed",
    "2-1": "Number Variable",
    "2-2": "The minimum speed required for the entity to stick. - m/s",
    "3-0": "Only Under Part",
    "3-1": "Transform Part Variable",
    "3-2": "Only if collided under this part",
    "4-0": "Stuck To",
    "4-1": "Bool Variable",
    "4-2": " - ReadOnly",
    "5-0": "Stuck To Entity",
    "5-1": "Entity Variable",
    "5-2": " - ReadOnly",
    "6-0": "Stuck To World",
    "6-1": "Vector3 Variable",
    "6-2": " - ReadOnly",
    "7-0": "Stuck To Anchor",
    "7-1": "Vector3 Variable",
    "7-2": " - ReadOnly",
    "8-0": "Stuck To Connected Anchor",
    "8-1": "Vector3 Variable",
    "8-2": " - ReadOnly"
  },
  "cols": 3,
  "rows": 9
}
[/block]