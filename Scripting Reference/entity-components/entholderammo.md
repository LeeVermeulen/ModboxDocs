---
title: "EntHolderAmmo"
slug: "entholderammo"
hidden: false
createdAt: "2020-11-10T21:51:07.049Z"
updatedAt: "2021-06-18T01:37:49.642Z"
---
**Holder Ammo**
Holds Ammo Container entities. Reloadable / removable

ID: EntHolderAmmo
Required By: [Holder Ammo Refiller](doc:entholderammorefiller)
Base Type: [Holder](doc:entholder)

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
    "1-0": "Set Starting Ammo Amount",
    "1-1": "Bool Variable",
    "1-2": "",
    "2-0": "Start Ammo Amount",
    "2-1": "Number Variable",
    "2-2": "Defaults to 10 - x",
    "3-0": "Removable",
    "3-1": "Bool Variable",
    "3-2": "",
    "4-0": "Default Entity",
    "4-1": "Entity Asset Variable",
    "4-2": "Entity asset the holder will create and start with",
    "5-0": "Scale Default Entity",
    "5-1": "Bool Variable",
    "5-2": "",
    "6-0": "Holding",
    "6-1": "Entity Variable",
    "6-2": "Entity held by holder",
    "7-0": "Holder Position",
    "7-1": "Transform Part Variable",
    "7-2": ""
  },
  "cols": 3,
  "rows": 8
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
    "0-0": "Held Ammo Container",
    "0-1": "Ammo Container",
    "0-2": ""
  },
  "cols": 3,
  "rows": 1
}
[/block]