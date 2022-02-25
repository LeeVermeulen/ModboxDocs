---
title: "EntAnimationInModel"
slug: "entanimationinmodel"
hidden: false
createdAt: "2020-11-10T22:11:20.001Z"
updatedAt: "2021-06-18T01:35:57.516Z"
---
**Animation In Model**
Plays Animation component in the Entity model, if any exist

ID: EntAnimationInModel
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
    "0-0": "Animation Name",
    "0-1": "Text Options Variable",
    "0-2": "Name of the animation to be played.",
    "1-0": "Animation Speed",
    "1-1": "Number Variable",
    "1-2": "Speed of the current animation playing. - Defaults to 1 - x",
    "2-0": "Animation Fade Length",
    "2-1": "Number Variable",
    "2-2": "Animation fade length in seconds when switching animations. - Defaults to 0.3 - s",
    "3-0": "Animation Wrap Mode",
    "3-1": "Enum Variable<Wrap Mode>",
    "3-2": "Wrap Mode of the current animation playing.",
    "4-0": "Animation Playing",
    "4-1": "Bool Variable",
    "4-2": ""
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
    "0-0": "Animations",
    "0-1": "Text List",
    "0-2": "Returns a list of available animation names"
  },
  "cols": 2,
  "rows": 1
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
    "0-0": "Animation",
    "0-1": "Animation",
    "0-2": ""
  },
  "cols": 3,
  "rows": 1
}
[/block]