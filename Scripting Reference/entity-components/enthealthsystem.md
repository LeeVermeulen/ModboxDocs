---
title: "EntHealthSystem"
slug: "enthealthsystem"
hidden: false
createdAt: "2020-11-10T21:59:49.767Z"
updatedAt: "2021-06-18T01:37:49.201Z"
---
**Health System**
Health system, dies when below 0 health

ID: EntHealthSystem
Required By: [Health System Damage Modifier](doc:enthealthsystemdamagemodifier), [Health System Health Bar](doc:enthealthsystemhealthbar)
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
    "0-0": "Health",
    "0-1": "Number Variable",
    "0-2": "hp",
    "1-0": "Take Damage",
    "1-1": "Bool Variable",
    "1-2": "If false the entity will not take damage. - Defaults to True",
    "2-0": "Flash On Hit",
    "2-1": "Bool Variable",
    "2-2": "",
    "3-0": "Heal Only To Start Health",
    "3-1": "Bool Variable",
    "3-2": "'Heal' will only heal to Start Health - Defaults to True",
    "4-0": "Start Health",
    "4-1": "Number Variable",
    "4-2": "Health that Playmode started with - hp"
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
    "0-0": "Reset Health",
    "0-1": "",
    "0-2": "",
    "1-0": "Do Damage(Number amount)",
    "1-1": "",
    "2-0": "Heal Health(Number amount)",
    "2-1": ""
  },
  "cols": 2,
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
    "0-0": "Health Percentage",
    "0-1": "Number",
    "0-2": "Percentage of health to Start health"
  },
  "cols": 3,
  "rows": 1
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
    "0-0": "On Damaged(Damage Info damage)",
    "0-1": ""
  },
  "cols": 2,
  "rows": 1
}
[/block]