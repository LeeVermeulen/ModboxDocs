---
title: "Prefabs"
slug: "prefabs"
hidden: false
createdAt: "2020-05-25T05:23:21.475Z"
updatedAt: "2021-06-14T17:37:40.439Z"
---
* MB Prefabs can be created in Edit mode out of 1 or more Entities.
* Prefabs are then a 'Entity Asset', and can be created like any other Entity asset. They can be placed in levels, set as the <<glossary:Player Avatar>> , or shot from guns as a projectile.
* Prefabs made in Modbox are sometimes called 'MB Prefabs' to differentiate them from 'Unity Prefabs' made from Unity GameObjects. They have a lot of the same functionality as Unity Prefabs, but are made entirely from Modbox Entities
* Use the 'Prefab Tool' to create prefabs ingame as a VR / Screen player. To create a Prefab in the [Desktop Editor](doc:desktop-editor), select 1 or more entities and use the 'Create Prefab' button at the top.
* Prefabs, like any other asset created ingame, can be saved locally or online and shared on Steam Workshop with other players. 
* Assets (such as models, materials, sounds, MBScripts) can be included in Prefabs.
* After editing a Prefab, 'Apply Changes' can be used to save changes to the saved prefab, which will update all other versions of that prefab in the world.
* Prefabs can include other prefabs inside them.
[block:image]
{
  "images": [
    {
      "image": [
        "https://files.readme.io/d69e650-PrefabOptions.png",
        "PrefabOptions.png",
        970,
        575,
        "#294a55"
      ],
      "caption": "When a value is set by the Prefab on a Entity, a Green bar is shown beside the value. If it's different than the Prefab value the bar is yellow.",
      "sizing": "80"
    }
  ]
}
[/block]

[block:api-header]
{
  "title": "Hierarchy Mode"
}
[/block]
When in Hierarchy Mode, Entities added are automatically added inside the current Prefab. There will also be a 'Apply Changes' option after exiting Hierarchy mode.