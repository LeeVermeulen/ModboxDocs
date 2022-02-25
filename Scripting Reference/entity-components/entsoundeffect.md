---
title: "EntSoundEffect"
slug: "entsoundeffect"
hidden: false
createdAt: "2020-11-10T21:51:06.809Z"
updatedAt: "2021-06-18T01:38:01.945Z"
---
**Sound Effect**
Plays audio clip assets

ID: EntSoundEffect
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
    "0-0": "Paused",
    "0-1": "Bool Variable",
    "0-2": "",
    "1-0": "Audioclip",
    "1-1": "Audioclip Variable",
    "1-2": "",
    "2-0": "Volume",
    "2-1": "Number Variable",
    "2-2": "x",
    "3-0": "Loop",
    "3-1": "Bool Variable",
    "3-2": "",
    "4-0": "Pitch",
    "4-1": "Number Variable",
    "4-2": "Defaults to 1",
    "5-0": "Play2d",
    "5-1": "Bool Variable",
    "5-2": "Will set sound to always play the same volume regardless of distance",
    "6-0": "Linear Roll Off",
    "6-1": "Bool Variable",
    "6-2": "Sound will roll off linear rather than logarithmic - so its louder from far away"
  },
  "cols": 3,
  "rows": 7
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
    "0-0": "Preview Sound",
    "0-1": "",
    "0-2": "",
    "1-0": "Play Once()",
    "1-1": ""
  },
  "cols": 2,
  "rows": 2
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
    "0-0": "Play Time",
    "0-1": "Number",
    "0-2": "",
    "1-0": "Is Playing",
    "1-1": "Bool",
    "1-2": ""
  },
  "cols": 3,
  "rows": 2
}
[/block]