---
title: "AssetPhysicsMaterial"
slug: "assetphysicsmaterial"
hidden: false
createdAt: "2020-11-10T21:34:57.228Z"
updatedAt: "2021-06-18T01:44:18.554Z"
---
**Physics Material**
Physics Material Asset sets a Entity physics properties - including it's mass, it's Physics Sound Type, and on damage/collision effects

ID: AssetPhysicsMaterial
Base Type: [Mod Asset](doc:modasset)

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
    "0-0": "Density",
    "0-1": "Number Variable",
    "0-2": "Mass of entities will be their volume X density - kg/m3",
    "1-0": "Physics Sound Type",
    "1-1": "Physics Sound Type Variable",
    "1-2": "",
    "2-0": "Break On Damage",
    "2-1": "Number Variable",
    "2-2": "hp",
    "3-0": "Break On Impact Speed",
    "3-1": "Number Variable",
    "3-2": "m/s",
    "4-0": "Break Effect",
    "4-1": "Effect Variable",
    "4-2": "Effect done on Entity breaking, or a big broken piece breaking",
    "5-0": "Damage Effect",
    "5-1": "Effect Variable",
    "5-2": "Effect when damage is done - from HitDamage entity / projectile / hitscan",
    "6-0": "Static Friction",
    "6-1": "Number Variable",
    "6-2": "The friction used when an object is laying still on a surface - x",
    "7-0": "Dynamic Friction",
    "7-1": "Number Variable",
    "7-2": "The friction used when already moving.  - x",
    "8-0": "Friction Combine",
    "8-1": "Enum Variable<Physic Material Combine>",
    "8-2": "How the friction of two colliding objects is combined",
    "9-0": "Bounciness",
    "9-1": "Number Variable",
    "9-2": "0 will not bounce - 1 will bounce with zero loss of energy - x",
    "10-0": "Bounciness Combine",
    "10-1": "Enum Variable<Physic Material Combine>",
    "10-2": "How the bounciness of two colliding objects is combined"
  },
  "cols": 3,
  "rows": 11
}
[/block]


Attributes:
UnityEngine.CreateAssetMenuAttribute
ModboxMain.MBTypeAssetCreateOptionAttribute