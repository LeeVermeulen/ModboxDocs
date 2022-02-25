---
title: "EntGrabBodySettings"
slug: "entgrabbodysettings"
hidden: false
createdAt: "2021-06-18T01:37:49.482Z"
updatedAt: "2021-06-18T01:37:49.483Z"
---
**Grab Body Settings**
Adds player grab settings that apply to entire physics body

ID: EntGrabBodySettings
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
    "0-0": "Ignore Weight",
    "0-1": "Bool Variable",
    "0-2": "Will allow easy grabbing and ignore the physics bodies weight",
    "1-0": "No Grabbing",
    "1-1": "Bool Variable",
    "1-2": "",
    "2-0": "Is Grabbed",
    "2-1": "Bool Variable",
    "2-2": " - ReadOnly"
  },
  "cols": 3,
  "rows": 3
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
    "0-0": "Grabbed By(Entity otherEntity, Entity ourEntity)",
    "0-1": "",
    "1-0": "Released By(Entity otherEntity, Entity ourEntity)",
    "1-1": ""
  },
  "cols": 2,
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
    "0-0": "Can Entity Grab(Entity otherEntity, Entity ourEntity)",
    "0-1": "Bool",
    "0-2": ""
  },
  "cols": 3,
  "rows": 1
}
[/block]