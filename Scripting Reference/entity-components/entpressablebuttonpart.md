---
title: "EntPressableButtonPart"
slug: "entpressablebuttonpart"
hidden: false
createdAt: "2020-11-10T21:51:07.013Z"
updatedAt: "2021-06-18T01:37:56.458Z"
---
**Pressable Button Part**
Fires an event when the pressable part is pressed.

ID: EntPressableButtonPart
Requires Components: [Pressable Part](doc:entpressablepart)
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
    "0-0": "Button Is Down",
    "0-1": "Bool Variable",
    "0-2": " - ReadOnly",
    "1-0": "Button Down On Collision",
    "1-1": "Bool Variable",
    "1-2": "Pushes the button down on colliding with something. This will only work if the pushable part is a transform underneath this entity. - Defaults to True",
    "2-0": "Button Down Time",
    "2-1": "Number Variable",
    "2-2": "Defaults to 1 - s",
    "3-0": "Button Down Offset",
    "3-1": "Vector3 Variable",
    "3-2": "Amount button will go down on pressed."
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
    "0-0": "Push Button",
    "0-1": "",
    "0-2": ""
  },
  "cols": 2,
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
    "0-0": "Button Down(Entity pressedButton)",
    "0-1": ""
  },
  "cols": 2,
  "rows": 1
}
[/block]