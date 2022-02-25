---
title: "Creating Entities"
slug: "advanced-mbscript"
hidden: false
createdAt: "2020-05-28T16:16:54.071Z"
updatedAt: "2021-06-17T20:14:00.998Z"
---
* Use the **Create** line to create entities. There are a few Create options like a new Entity from a Asset, or clone a existing entity.

* Create lines have options to set the start position of the entity / rotation. They also have options creating the Entity and staying in it's 'Edit Mode' state, or starting as Disabled

* The Create line creates a new local variable. So you could Create a Entity as disabled or in edit mode, change some of it's values, then turn Disabled off or turn on it's play mode.
[block:image]
{
  "images": [
    {
      "image": [
        "https://files.readme.io/2718897-createEntity.png",
        "createEntity.png",
        735,
        327,
        "#1b3f4f"
      ],
      "caption": "The Entity is cloned and is set to 'Edit Mode'. A 'HealthSystem' component is added, it's health set to 20, then Playmode is turned on for it."
    }
  ]
}
[/block]