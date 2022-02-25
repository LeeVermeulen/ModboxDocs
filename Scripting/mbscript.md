---
title: "MBScript"
slug: "mbscript"
hidden: false
createdAt: "2020-05-25T05:28:15.021Z"
updatedAt: "2021-06-17T19:55:01.727Z"
---
MBScript is the visual scripting system for the game creation tool [Modbox](http://www.modboxgame.com). It was designed instead of using a existing text scripting language (like Lua/Javascript) for a few reasons:
* To allow designers to create complex gameplay / AI with drag and drop editing (No syntax errors)
* Can be edited with Keyboard+Mouse, in VR \ AR, with Touch on a mobile device, or with a Gamepad.
* Designed from the start to work online. All code runs online automatically so designers never have to think about networking state
* All changes made to MBScript code are also synced online to other players in real time - and can be edited while playing.
* Unlike node based visual scripting (like Blueprints / Playmaker), MBScript can be switched from visual mode to text mode at any time. A integrated VSCode like text editor (Monaco) is included with Modbox.
* Code can be copied and pasted between the node based [Wiring](doc:wiring) system, which uses MBScript
* It's event based - with events being any variable changes or ingame events on any entity in the world - so MBScript code can be easily hooked into by other scripts / mods.
* Uses the C# type system to show the correct options and validate the drag and drop blocks
[block:html]
{
  "html": "<iframe src='https://gfycat.com/ifr/fearfulshowyisabellineshrike' frameborder='0' scrolling='no' allowfullscreen width='640' height='404'></iframe>"
}
[/block]
Here a MBScript asset is created to have the Entity 'Die' on Collision if the collision speed is over the 'Min Speed to Break' number variable. It also Prints the name of the Entity it collided with.
[block:api-header]
{
  "title": "Creating Scripts"
}
[/block]
* MBScript assets can be created with the Edit Entity Desktop Window or the Edit VR Tool. Each asset creates a new <<glossary:Entity Component>> type. MBScript Assets can be included in Entity <<glossary:Prefab>>. 

* MBScript can be edited/run at anytime (Running in edit mode can be useful for creating Editor tools / operations. Editing in play mode is a easy way to test changes.)

* MBScript is also used to create [Game Managers](doc:game-managers) - which are MBScript assets that are added to the world automatically, and easily accessed by other scripts (like [Singletons ](https://en.wikipedia.org/wiki/Singleton_pattern))
[block:api-header]
{
  "title": "Video Tutorials"
}
[/block]

[block:embed]
{
  "html": "<iframe class=\"embedly-embed\" src=\"//cdn.embedly.com/widgets/media.html?src=https%3A%2F%2Fwww.youtube.com%2Fembed%2FYkO7VgpF4-o%3Fstart%3D7%26feature%3Doembed%26start%3D7&display_name=YouTube&url=https%3A%2F%2Fwww.youtube.com%2Fwatch%3Fv%3DYkO7VgpF4-o&image=https%3A%2F%2Fi.ytimg.com%2Fvi%2FYkO7VgpF4-o%2Fhqdefault.jpg&key=f2aa6fc3595946d0afc3d76cbbd25dc3&type=text%2Fhtml&schema=youtube\" width=\"854\" height=\"480\" scrolling=\"no\" title=\"YouTube embed\" frameborder=\"0\" allow=\"autoplay; fullscreen\" allowfullscreen=\"true\"></iframe>",
  "url": "https://www.youtube.com/watch?v=YkO7VgpF4-o&t=7s&ab_channel=LeeVermeulen",
  "title": "Modbox - Scripting Tutorial/Intro",
  "favicon": "https://www.youtube.com/s/desktop/ebcf1b0f/img/favicon.ico",
  "image": "https://i.ytimg.com/vi/YkO7VgpF4-o/hqdefault.jpg"
}
[/block]

[block:api-header]
{
  "title": "Events"
}
[/block]
* MBScript code runs on **Events**, which allows for running code based on any event happening on the Entity or in the world (such as a variable changes value, or a world event happens like a player joins).

[block:image]
{
  "images": [
    {
      "image": [
        "https://files.readme.io/774e0ad-SimpleMBScript.png",
        "SimpleMBScript.png",
        621,
        355,
        "#173f4f"
      ],
      "caption": "A Event line is added for the 'Start' event - printing 'Hello World' to the screen.\n\nA new variable 'SwitchColors' is added, with default value 'True'. Here the Entity's Color will be set a random color every Update if 'SwitchColors' is True",
      "sizing": "80"
    }
  ]
}
[/block]
The 'On' lines add *Event Lines* to run code on events. You can then add other code line types to set values / do operations:
- **Set **- Set a variable's value
- **Do** - Do a method / operation / or event
- **If** - Run code if a condition is true. Can then add *Else* lines
- **Print** - Print a value to the screen, useful for quick testing
- **ForEach **- Run code on a list. “Do this to everything in this set". Can run ‘ForEach Entity in the world change it’s material to Wood’
- **Wait** - Wait a set amount of time before running next code
There are a few other line types: ‘**Local**’ for temporary variables, **Return **to stop running code and return from an event, **For** to do a 'for' loop a set number of times, and **While** to keep looping while a condition is True

Code can run on multiple events and have conditions setting when it runs:
[block:image]
{
  "images": [
    {
      "image": [
        "https://files.readme.io/b9e7def-MBScriptEventCondition.png",
        "MBScriptEventCondition.png",
        1343,
        307,
        "#193c4c"
      ],
      "sizing": "smart",
      "caption": "Here the first event line runs if the Entity's name changed, or if it just started.\nThe second event line runs when a Collision happens, and if the collision was with a Animated Humanoid"
    }
  ]
}
[/block]

[block:api-header]
{
  "title": "Selecting Variables"
}
[/block]
After adding a code line you use the dropdowns to choose a variable or set a value.

After selecting a variable it will show if it still needs the expected type.

[block:image]
{
  "images": [
    {
      "image": [
        "https://files.readme.io/b6db279-ExpectedType.png",
        "ExpectedType.png",
        347,
        62,
        "#43555b"
      ],
      "sizing": "80",
      "caption": "The ‘If’ code line needs a ‘True/False’ value, so after selecting ‘Name’ (which is a Text variable) you still need to return a True/False value, so the ‘Select’ is shown to select an option inside the Name text."
    }
  ]
}
[/block]

[block:image]
{
  "images": [
    {
      "image": [
        "https://files.readme.io/2721401-ExpectedType2.png",
        "ExpectedType2.png",
        451,
        60,
        "#1b3f4e"
      ],
      "caption": "‘Contains’ was selected to check if the name contains ‘Bob’. So if this is True the code inside the ‘If’ line will run.",
      "sizing": "80"
    }
  ]
}
[/block]
The ‘+’ at the end of the line can be used to continue the line with another operation. So because ‘Contains’ returns a True/False, you can then hit the ‘+’ button and select ‘IsFalse’ to invert that return value:
[block:image]
{
  "images": [
    {
      "image": [
        "https://files.readme.io/e2d779f-ExpectedType3.png",
        "ExpectedType3.png",
        560,
        62,
        "#1c3f4f"
      ],
      "sizing": "80",
      "caption": "The code under this “If’ line will now run if the name doesn’t contain ‘Bob’."
    }
  ]
}
[/block]
You can keep adding operations like this. Here the ‘Y’ part of the entity’s scale is selected, and set to the same Y value plus a random value:
[block:image]
{
  "images": [
    {
      "image": [
        "https://files.readme.io/412b714-ExpectedType4.png",
        "ExpectedType4.png",
        986,
        67,
        "#1d3b4a"
      ],
      "sizing": "smart",
      "caption": ""
    }
  ]
}
[/block]

[block:api-header]
{
  "title": "Variable Options"
}
[/block]
When selecting a variable in MBScript you select from either:
* Variables created in the Script
* Local variables (added with Local line or as parameters to the Event)
* Components on the Entity and their variables (like it's Name in the Main component, or Mass in the Physics component)
* Variables in the World (like Gravity, or list of all Material Assets)
* Or Functions - that just return a value. Like 'Func.Random.Value' or 'Func.Mathf.Cos('
[block:api-header]
{
  "title": "Tooltips"
}
[/block]
Hover over a icon to see a description of the variable and it's value.

[block:image]
{
  "images": [
    {
      "image": [
        "https://files.readme.io/b323c85-Hover.png",
        "Hover.png",
        727,
        225,
        "#71802d"
      ],
      "sizing": "80"
    }
  ]
}
[/block]

[block:image]
{
  "images": [
    {
      "image": [
        "https://files.readme.io/68cc45e-Hover2.png",
        "Hover2.png",
        727,
        285,
        "#294c48"
      ],
      "caption": "You can also hover to see the Value results at any time. Here hovering over Divide shows the value of the Health variable divided by 20",
      "sizing": "80"
    }
  ]
}
[/block]

[block:api-header]
{
  "title": "Operations"
}
[/block]
To change a variable value the Set line can be used to set to a new value (with "Set X to Y"). It can also be useful to do operations directly on the variable:
[block:image]
{
  "images": [
    {
      "image": [
        "https://files.readme.io/75c31b2-EaseTo.PNG",
        "EaseTo.PNG",
        669,
        160,
        "#17404f"
      ],
      "caption": "'Do' can be used to run operations on variables. Here 1 is added to the Number1 variable\n\nThe second line shows using the \"Ease To\" operation to change a color variable over time. This can be run just once to have it slowly turn color to black."
    }
  ]
}
[/block]

[block:api-header]
{
  "title": "Lists and Queries"
}
[/block]
The 'ForEach' line can be used to iterate through lists - like the 'All Entities' list in the world.
[block:image]
{
  "images": [
    {
      "image": [
        "https://files.readme.io/04d2962-ForEachExam.png",
        "ForEachExam.png",
        587,
        125,
        "#203a49"
      ],
      "caption": "Go through all entities in the world and print their position",
      "sizing": "80"
    }
  ]
}
[/block]

[block:image]
{
  "images": [
    {
      "image": [
        "https://files.readme.io/b116ed7-ForEachExam2.png",
        "ForEachExam2.png",
        715,
        125,
        "#1e414f"
      ],
      "caption": "Go through all Primitive components in the world and print their Material value",
      "sizing": "80"
    }
  ]
}
[/block]

[block:image]
{
  "images": [
    {
      "image": [
        "https://files.readme.io/ce3c344-Lambda.PNG",
        "Lambda.PNG",
        920,
        104,
        "#1d3b4a"
      ],
      "caption": "You can also do queries on lists (like C#'s LINQ) using 'lambda'.\nHere it prints the name of all Entities with a mass greater than 1.\nCould also keep adding to this, adding a 'OrderBy' to order it by mass.",
      "sizing": "80"
    }
  ]
}
[/block]

[block:api-header]
{
  "title": "Editing"
}
[/block]
* Code lines can be dragged by moving the drag handle. Multiple lines can be selected and moved at once. Variables and values can also be dragged to copy them.
* Right click can be used to copy and paste MBScript (which just copies it to the Clipboard as text)

[block:api-header]
{
  "title": "Text Editing"
}
[/block]
* MBScript can be copy and pasted as text.
* At any time you can switch to text mode to edit, with autocomplete for variable names and immediate error updates. 

Here is the same script switched to text mode and edited, checking if the Entity has a 'Primitive Component' set on it, and if it does it prints the value of the Entity's <<glossary:Physics Material Asset>> : 
[block:html]
{
  "html": "<iframe src='https://gfycat.com/ifr/peskytinyharpyeagle' frameborder='0' scrolling='no' allowfullscreen width='640' height='404'></iframe>"
}
[/block]