---
title: "EntGrabSettings"
slug: "entgrabsettings"
hidden: false
createdAt: "2020-11-10T22:11:20.247Z"
updatedAt: "2021-06-18T01:37:49.268Z"
---
**Grab Settings**
Adds player grab settings for picking up with VR hands / screen cursor - No grabbing, Is Grabbed

ID: EntGrabSettings
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
    "0-0": "Grabbed By(Entity otherEntity)",
    "0-1": "",
    "1-0": "Released By(Entity otherEntity)",
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
    "0-0": "Can Entity Grab(Entity otherEntity)",
    "0-1": "Bool",
    "0-2": "Set with a event if a Entity can grab"
  },
  "cols": 3,
  "rows": 1
}
[/block]