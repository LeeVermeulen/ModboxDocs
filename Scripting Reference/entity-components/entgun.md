---
title: "EntGun"
slug: "entgun"
hidden: false
createdAt: "2020-11-10T22:11:20.205Z"
updatedAt: "2021-06-18T01:37:49.242Z"
---
**Gun**
Fires a Projectile

ID: EntGun
Required By: [Gun Animation On Fire](doc:entgunanimationonfire), [Gun Chargable](doc:entgunchargable), [Gun Charge With Pullable Part](doc:entgunchargewithpullablepart), [Gun Cycle Shot Position](doc:entguncycleshotposition), [Gun Loadable](doc:entgunloadable), [Gun Shell Position](doc:entgunshellposition), [Gun Shoot On Releasing Pullable Part](doc:entgunshootonreleasingpullablepart), [Gun Shoot On Trigger](doc:entgunshootontrigger), [Minigun Shoot With Rotatable Part](doc:entminigunshootwithrotatablepart)
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
    "0-0": "Projectile",
    "0-1": "Projectile Variable",
    "0-2": "Projectile asset that will be fired",
    "1-0": "Shot Position",
    "1-1": "Transform Part Variable",
    "1-2": "Transform to fire projectile from",
    "2-0": "Take Ammo",
    "2-1": "Bool Variable",
    "2-2": "If firing should require Ammo from a Ammo Container",
    "3-0": "Next Shot",
    "3-1": "Play Time Variable",
    "3-2": "Time till next shot, set by projectile asset refire time -  - ReadOnly",
    "4-0": "Using Ammo Container",
    "4-1": "Entity Component Variable<Ammo Container>",
    "4-2": "The AmmoContainer this Gun is using. Based on if it uses Ammo and it's Projectile - will find any AmmoContainer on the Entity/Body -  - ReadOnly"
  },
  "cols": 3,
  "rows": 5
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
    "0-0": "Shoot",
    "0-1": "",
    "0-2": "Shoot Projectile",
    "1-0": "Shoot With Charge",
    "1-1": "",
    "1-2": "Shoot Projectile with a set Charge amount",
    "2-0": "Shoot With Charge At(Number charge, Vector3 worldPosition, Vector3 worldRotation)",
    "2-1": "Shoot Projectile at a specific position/angle"
  },
  "cols": 2,
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
    "0-0": "Gun Shot()",
    "0-1": "On Projectile fired",
    "1-0": "On Projectile Hit(Projectile Hit Info info)",
    "1-1": "Called when a projectile from this gun hit something",
    "2-0": "Next Shot Lapsed()",
    "2-1": "Called when Next Shot time Lapses"
  },
  "cols": 2,
  "rows": 3
}
[/block]