---
title: "EntHealthSystemDamageModifier"
slug: "enthealthsystemdamagemodifier"
hidden: false
createdAt: "2021-06-18T01:37:49.237Z"
updatedAt: "2021-06-18T01:37:49.237Z"
---
**Health System Damage Modifier**
Adds option to multiply Damage, or ignore/change it with a return event before it's applied

ID: EntHealthSystemDamageModifier
Requires Components: [Health System](doc:enthealthsystem)
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
    "0-0": "Damage Multiply",
    "0-1": "Number Variable",
    "0-2": "Defaults to 1 - x"
  },
  "cols": 3,
  "rows": 1
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
    "0-0": "Modify Damage(Damage Info damage)",
    "0-1": "Number",
    "0-2": "Modify the damage amount - return 0 to do no damage",
    "1-0": "Ignore Damage(Damage Info damage)",
    "1-1": "Bool",
    "1-2": "Modify the damage amount - return 0 to do no damage"
  },
  "cols": 3,
  "rows": 2
}
[/block]


Attributes:
ModboxMain.MBOldIDAttribute