---
title: "Wiring"
slug: "wiring"
hidden: false
createdAt: "2020-05-25T06:35:56.098Z"
updatedAt: "2020-10-31T14:13:39.004Z"
---
* The Wiring system is a visual scripting system for connecting entities together to run logic and scripting, similar to other node scripting systems like Unreal Blueprints / Unity Playmaker

* It uses the same variables and options as [MBScript](doc:mbscript), but can useful for quickly making connections between Entities in a visual way. Wiring could be used to connect a Switch to a Door to open it ingame, while [MBScript](doc:mbscript) should be used to make reusable components / complex AI

* Use the Wiring Tool, or open the Wiring Desktop Window. Select a Entity to start Wiring from it.

* To trigger **Actions** (such as changing a variable), select the **Events ** to run the Wiring on. You can also select **Conditions** that need to be True for the Wiring to happen.
* **Events** can be Event variables (like 'Start' and 'Update'), or when a variable value changes (like it's Color or Scale), or when a method is run on a Entity (like 'Die')

[block:image]
{
  "images": [
    {
      "image": [
        "https://files.readme.io/930f968-Wiring_Event.png",
        "Wiring_Event.png",
        2897,
        1262,
        "#2c4d55"
      ],
      "caption": "Wiring a Lever Entity to a Spin Joint to turn it on",
      "sizing": "80"
    }
  ]
}
[/block]
* On starting to Wiring a Entity to another one we select from the Components in the selected Entity, or the Entity it's Wired to.

* In the above image the Lever is wiring to the Spin Joint - so it's showing [Entity Components](doc:components-1) options that are in the Lever.

[block:image]
{
  "images": [
    {
      "image": [
        "https://files.readme.io/ad55843-WiringLeveer.PNG",
        "WiringLeveer.PNG",
        2996,
        1137,
        "#274952"
      ],
      "caption": "Here the Lever is wired to the Spin Joint, to set it's 'Motor' variable to True in it's HingeJointMotor component",
      "sizing": "80"
    }
  ]
}
[/block]

[block:api-header]
{
  "title": "Actions"
}
[/block]
On hitting the + button beside "Actions" you can select to add a new action line:
- **Set **- Set a variable's value
- **Do** - Do a method / operation / or event
- **Print** - Print a value to the screen, useful for quick testing

These are the same as [MBScript](doc:mbscript) code lines.
[block:api-header]
{
  "title": "Advanced"
}
[/block]
* All MBScript variables and options are available to Wiring - including [World Settings](doc:world-settings)  and all functions / members / extensions of a variable.
* Entities can also be Wired to themselves to change values and respond to events
* Wiring can also include 'local variables' like [MBScript](doc:mbscript). New local variables can be set with the **Local** line
* The **Create** line spawns a new Entity, and shows it as a local variable. You can then set variables / do events on this new spawned Entity. 

Here is a example of Wiring a Cube to itself, to change the color of Entities it collides with (if it collides with them at a speed greater than 1):
[block:html]
{
  "html": "<iframe src='https://gfycat.com/ifr/TidySeriousCaiman' frameborder='0' scrolling='no' allowfullscreen width='640' height='404'></iframe>"
}
[/block]
Here wiring is set to run on the 'On Collision' event on a Cube. The 'collisionInfo' is a local variable set by the collision event. It has a condition setting that it's collision speed must be above 4 - and if it is, then it sets the Color on the Entity it hit to Black.

 * The Wiring data will be saved in the Entity it started with. So Prefabs made of that entity (or clones) will clone the Wiring data