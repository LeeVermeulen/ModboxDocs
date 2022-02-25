---
title: "EntAmmoContainer"
slug: "entammocontainer"
hidden: false
createdAt: "2020-11-10T22:11:20.124Z"
updatedAt: "2021-06-18T01:35:57.489Z"
---
**Ammo Container**
Contains ammo for Gun component

ID: EntAmmoContainer
Required By: [Ammo Container Hide Ammo Parts](doc:entammocontainerhideammoparts), [Ammo Container Scale Part With Ammo](doc:entammocontainerscalepartwithammo)
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
    "0-0": "Ammo Type",
    "0-1": "Projectile Ammo Variable",
    "0-2": "",
    "1-0": "Ammo",
    "1-1": "Number Variable",
    "1-2": "ammo",
    "2-0": "Remove Entity On No Ammo",
    "2-1": "Bool Variable",
    "2-2": "If true automatically removes the Entity when ammo is 0 or below"
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
    "0-0": "Starting Ammo",
    "0-1": "Number",
    "0-2": "Ammo set before starting play mode"
  },
  "cols": 3,
  "rows": 1
}
[/block]