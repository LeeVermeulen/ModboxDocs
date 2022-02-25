---
title: "EntGunChargable"
slug: "entgunchargable"
hidden: false
createdAt: "2020-11-10T22:11:20.137Z"
updatedAt: "2021-06-18T01:37:49.323Z"
---
**Gun Chargable**
Adds a CurrentCharge number, Charging bool, and ShootWithCharge option for a gun

ID: EntGunChargable
Requires Components: [Gun](doc:entgun)
Required By: [Gun Chargable Charge Effect](doc:entgunchargablechargeeffect), [Gun Charge With Pullable Part](doc:entgunchargewithpullablepart), [Gun Charge With Trigger](doc:entgunchargewithtrigger)
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
    "0-0": "Current Charge",
    "0-1": "Number Variable",
    "0-2": "x",
    "1-0": "Charge Up Speed",
    "1-1": "Number Variable",
    "1-2": "How fast to increase CurrentCharge when Charging is true - x",
    "2-0": "Charging",
    "2-1": "Bool Variable",
    "2-2": "",
    "3-0": "Charge Up Sound",
    "3-1": "Audioclip Variable",
    "3-2": "Sound to play on charging"
  },
  "cols": 3,
  "rows": 4
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
    "0-0": "Shoot With Charge",
    "0-1": "",
    "0-2": "Shoot gun with the current charge"
  },
  "cols": 2,
  "rows": 1
}
[/block]