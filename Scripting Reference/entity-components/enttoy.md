---
title: "EntToy"
slug: "enttoy"
hidden: false
createdAt: "2020-11-10T21:51:06.795Z"
updatedAt: "2021-06-18T01:38:01.999Z"
---
**Toy**
Entities that can be picked up and held

ID: EntToy
Required By: [Toy Face Pulled Direction](doc:enttoyfacepulleddirection), [Toy Active Parts On Held](doc:enttoyactivepartsonheld), [Toy Can Entity Hold](doc:enttoycanentityhold), [Toy Disable Dropping](doc:enttoydisabledropping), [Toy Held Animation On Trigger](doc:enttoyheldanimationontrigger), [Toy Held Animation Throw On Trigger](doc:enttoyheldanimationthrowontrigger), [Toy Shield](doc:enttoyshield), [Holder Attachment Scope](doc:entholderattachmentscope)
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
    "0-0": "Held By Hand",
    "0-1": "Entity Component Variable<Holder Hand>",
    "0-2": " - ReadOnly",
    "1-0": "Can Hold",
    "1-1": "Bool Variable",
    "1-2": "Defaults to True",
    "2-0": "Toy Hold Position",
    "2-1": "Transform Part Variable",
    "2-2": ""
  },
  "cols": 3,
  "rows": 3
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
    "0-0": "Is Held",
    "0-1": "Bool",
    "0-2": ""
  },
  "cols": 3,
  "rows": 1
}
[/block]