---
title: "UI Editing"
slug: "building-ui"
hidden: false
createdAt: "2020-05-25T05:23:20.718Z"
updatedAt: "2021-06-21T22:43:28.224Z"
---
* The 'Core UI' mod includes UI Entities which can be used to be build UI such as the player's HUD, menu screens, and other ingame displays.
* UI Entities have to be in a <<glossary:UI Canvas>> entity.

* The 'UI Canvas' can be set to 'Screen Overlay' mode - which will then show it on the Screen for all users (but not in VR player headsets). To create a HUD / UIScreen - a <<glossary:Prefab>> needs to be created of the canvas

[block:image]
{
  "images": [
    {
      "image": [
        "https://files.readme.io/940a050-UIEntities.PNG",
        "UIEntities.PNG",
        1184,
        657,
        "#274955"
      ],
      "caption": "A UI Canvas is placed in the world then the UI entities are added to it. Here a NumberBar is added to be used to display health."
    }
  ]
}
[/block]

[block:api-header]
{
  "title": "Alignment"
}
[/block]
* One important aspect of creating UI is setting the Alignment. By default UI entities align to the center - but when creating a HUD you might want to align to the bottom / top / right / left. This is important since the Canvas will be displayed at different sizes depending on the players resolution.
[block:image]
{
  "images": [
    {
      "image": [
        "https://files.readme.io/62a2821-Alignment.PNG",
        "Alignment.PNG",
        631,
        272,
        "#1c5368"
      ],
      "caption": "Can set the alignment in the 'UI Transform' component"
    }
  ]
}
[/block]

[block:api-header]
{
  "title": "UI Prefabs"
}
[/block]
* To create a HUD / UI Screen for users, create a [Prefabs](doc:prefabs) of the UI Canvas.

* To set this prefab as the default HUD for all players - set 'Default HUD' in 'Players' section of [Creation Settings](doc:creation-settings). This will then add that HUD to the player when they start playing.
* To add a HUD to a specific player - add a [EntPlayerHUD](doc:entplayerhud) component to the User/Avatar and set the prefab as 'UseCanvases' list

* The [Wiring](doc:wiring) system and [MBScript](doc:mbscript) can be used to control the UI and what it displays.
[block:api-header]
{
  "title": "UI Screens"
}
[/block]
* To create a <<glossary:UI Screen>> - in the 'Assets' screen create a new 'UI Screen Entity Canvas' asset. Then set it's 'Canvas Prefab' to the UI Prefab
* A UI Screen can be set to be 'Show In Menu Options' - so it will shown as a option when the user has their menu open
* UI Screens can be shown to a User through <<glossary:MBScript>> by using 'User.ShowScreen('
* In [Creation Settings](doc:creation-settings) - a UI Screen can be set as the 'Game Menu'. It will then show as a option to open while playing (as a input hint on the screen to open for screen players with Tab, or as a button on a VR controller)