---
title: "EntHitDamageCanDamageEntity"
slug: "enthitdamagecandamageentity"
hidden: false
createdAt: "2020-11-10T21:59:50.117Z"
updatedAt: "2021-06-18T01:37:49.668Z"
---
**Hit Damage Can Damage Entity**
Adds a return event to set if HitDamage should damage depending on the hit entity

ID: EntHitDamageCanDamageEntity
Requires Components: [Hit Damage](doc:enthitdamage)
Base Type: [Entity Component](doc:componententity)

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
    "0-0": "Can Damage Entity(Entity hitEntity, Number damage, Collision Info collisionInfo)",
    "0-1": "Bool",
    "0-2": "Returns if the damage should happen to the hit entity"
  },
  "cols": 3,
  "rows": 1
}
[/block]