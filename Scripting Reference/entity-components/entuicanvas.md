---
title: "EntUICanvas"
slug: "entuicanvas"
hidden: false
createdAt: "2020-11-10T21:51:06.851Z"
updatedAt: "2021-06-18T01:38:07.748Z"
---
**UI Canvas**
Canvas where UI entities can be placed under

ID: EntUICanvas
Required By: [GameOverScreen](doc:mbsgameoverscreen), [YouDiedScreen](doc:mbsyoudiedscreen)
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
    "0-0": "On User",
    "0-1": "Entity Component Variable<User>",
    "0-2": "The User this Canvas is on if this is on a player Screen / Tool -  - ReadOnly",
    "1-0": "On Player Avatar",
    "1-1": "Entity Component Variable<Player Avatar>",
    "1-2": "The Avatar this Canvas is on if this is on a player Screen / Tool. Will update to the User's current avatar if on a User -  - ReadOnly",
    "2-0": "Screen Overlay",
    "2-1": "Bool Variable",
    "2-2": "Canvas will overlay over the screen for all users. Will not show in VR/AR headset (Create a Prefab and set that as the HUD in Creation Settings for that)",
    "3-0": "Canvas Size",
    "3-1": "Vector2 Variable",
    "3-2": "",
    "4-0": "Show Border",
    "4-1": "Bool Variable",
    "4-2": "Defaults to True",
    "5-0": "Show Background",
    "5-1": "Bool Variable",
    "5-2": "Defaults to True",
    "6-0": "Interactable",
    "6-1": "Bool Variable",
    "6-2": "Allows users to interact with UI when in the world - Defaults to True",
    "7-0": "Background Color",
    "7-1": "Color Variable",
    "7-2": "",
    "8-0": "Test With Avatar In World",
    "8-1": "Bool Variable",
    "8-2": "Set this Canvas's PlayerAvatar to the first PlayerAvatar thats in the world as if this Cavnas was it's UI HUD"
  },
  "cols": 3,
  "rows": 9
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
    "0-0": "On UI Screen Canvas",
    "0-1": "UI Screen Canvas",
    "0-2": "The UI Screen canvas this canvas this is on if part of a UI Screen",
    "1-0": "Canvas Mode",
    "1-1": "UI Canvas Mode",
    "1-2": "The current state of the canvas - if it's in the World / In a Menu / Screen"
  },
  "cols": 3,
  "rows": 2
}
[/block]


Attributes:
ModboxMain.MBTypeComponentNoIngameAddingAttribute