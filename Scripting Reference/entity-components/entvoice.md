---
title: "EntVoice"
slug: "entvoice"
hidden: false
createdAt: "2020-11-10T21:51:06.818Z"
updatedAt: "2021-06-18T01:38:07.759Z"
---
**Voice**
Adds method to play Audioclip as voice

ID: EntVoice
Required By: [Voice Speech](doc:entvoicespeech)
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
    "0-0": "Volume",
    "0-1": "Number Variable",
    "0-2": "x",
    "1-0": "Pitch",
    "1-1": "Number Variable",
    "1-2": "Defaults to 1",
    "2-0": "Play2d",
    "2-1": "Bool Variable",
    "2-2": "Will set sound to always play the same volume regardless of distance",
    "3-0": "Linear Roll Off",
    "3-1": "Bool Variable",
    "3-2": "Voice audio will 'roll off' linearly rather than logarithmic so farther away players can hear",
    "4-0": "Is Speaking",
    "4-1": "Bool Variable",
    "4-2": " - ReadOnly"
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
    "0-0": "Play As Voice(Audio Clip clipAsset)",
    "0-1": "Plays a Audioclip coming from the Entity - will be used by any LipSync / Facial components"
  },
  "cols": 2,
  "rows": 1
}
[/block]