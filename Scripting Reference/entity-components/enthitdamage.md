---
title: "EntHitDamage"
slug: "enthitdamage"
hidden: false
createdAt: "2020-11-10T21:59:49.717Z"
updatedAt: "2021-06-18T01:37:49.555Z"
---
**Hit Damage**
Does damage on collision

ID: EntHitDamage
Required By: [Hit Damage Can Damage Entity](doc:enthitdamagecandamageentity), [Hit Damage Effect On Hit](doc:enthitdamageeffectonhit), [Hit Damage Part](doc:enthitdamagepart), [Hit Damage Scale Damage With Speed](doc:enthitdamagescaledamagewithspeed), [Hit Damage Set Hit Force](doc:enthitdamagesethitforce)
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
    "0-0": "Hit Damage Enabled",
    "0-1": "Bool Variable",
    "0-2": "Defaults to True",
    "1-0": "Damage Amount",
    "1-1": "Number Variable",
    "1-2": "hp",
    "2-0": "Damage Min Relative Speed",
    "2-1": "Number Variable",
    "2-2": "Minimum relative speed of collision needed to do damage - m/s",
    "3-0": "Damage Min Own Speed",
    "3-1": "Number Variable",
    "3-2": "Minimum speed this entity needs to be going to do damage - m/s"
  },
  "cols": 3,
  "rows": 4
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
    "0-0": "On Hit(Entity hitEntity, Number damage, Collision Info collisionInfo)",
    "0-1": ""
  },
  "cols": 2,
  "rows": 1
}
[/block]