---
title: "Editing Entities"
slug: "editing-entities"
hidden: false
createdAt: "2020-05-26T05:57:27.706Z"
updatedAt: "2020-06-24T13:30:35.455Z"
---
* Entity properties can be set with the Edit Tool, or the 'Edit Entity' desktop window.
* Entities are made of [Entity Components](doc:components-1) . There is always a 'Main' component which sets properties like the Entity name / if it's disabled, and a 'Transform' component which sets where it is in the world and what it's connected to.
* <<glossary:Entity Component>>s can be added to entities - which will also add of that components required components. Components are created with either [MBScript](doc:mbscript), or C# programming.
* [Prefabs](doc:prefabs) can be created made from 1 or more entities. Prefabs can then be used just like other Entity assets.
[block:api-header]
{
  "title": "Connections"
}
[/block]
Depending on the Entity type it might **Autoconnect** to other Entities. This can be turned off/on on the Entity.
If a Entity has a 'Physics' component it will have physics in play mode and a single physics body with anything it is connected to (including connected Entities without Physics component).
Physics is done by connections rather than a Hierarchy (which is the usual ways physics are done in other games).

[block:api-header]
{
  "title": "Edit mode Physics"
}
[/block]
Physics can be turned on for Entities in edit mode to have them collide with the environment / other entities when placing.
Gravity can also be turned on to have them fall to the ground (good for realistic placing of props).

[block:html]
{
  "html": "<iframe src='https://gfycat.com/ifr/QueasyImpassionedDromaeosaur' frameborder='0' scrolling='no' allowfullscreen width='640' height='404'></iframe>"
}
[/block]