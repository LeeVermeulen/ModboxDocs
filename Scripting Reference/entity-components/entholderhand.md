---
title: "EntHolderHand"
slug: "entholderhand"
hidden: false
createdAt: "2020-11-10T21:59:50.145Z"
updatedAt: "2021-06-18T01:37:49.616Z"
---
**Holder Hand**
Holds Entities as if held by a Hand

ID: EntHolderHand
Required By: [Holder Hands Dont Take Ammo](doc:entholderhandsdonttakeammo)
Base Type: [Holder](doc:entholder)
Base Of: [Holder Hand Animated](doc:entholderhandanimated), [Holder Hand Left Interface](doc:entholderhandleftinterface), [Holder Hand Right Interface](doc:entholderhandrightinterface), [Holder Hand VR](doc:entholderhandvr)

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
    "0-0": "Drop On Death",
    "0-1": "Bool Variable",
    "0-2": "If held entity should drop on death, otherwise will be removed",
    "1-0": "Default Entity",
    "1-1": "Entity Asset Variable",
    "1-2": "Entity asset the holder will create and start with",
    "2-0": "Scale Default Entity",
    "2-1": "Bool Variable",
    "2-2": "",
    "3-0": "Holding",
    "3-1": "Entity Variable",
    "3-2": "Entity held by holder",
    "4-0": "Holder Position",
    "4-1": "Transform Part Variable",
    "4-2": ""
  },
  "cols": 3,
  "rows": 5
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
    "0-0": "Is Left Hand",
    "0-1": "Bool",
    "0-2": ""
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
    "0-0": "Held Gun Fired()",
    "0-1": ""
  },
  "cols": 2,
  "rows": 1
}
[/block]