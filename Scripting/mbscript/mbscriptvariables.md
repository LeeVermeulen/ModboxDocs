---
title: "MBScript Variables"
slug: "mbscriptvariables"
hidden: false
createdAt: "2020-05-25T18:35:06.690Z"
updatedAt: "2021-06-17T20:44:28.808Z"
---
You can add Variables to the MBScript code which will then show in the Entity properties.
[block:image]
{
  "images": [
    {
      "image": [
        "https://files.readme.io/bead24d-AddedVariable.png",
        "AddedVariable.png",
        1090,
        202,
        "#214555"
      ],
      "caption": "'OtherEntity' is a Entity Variable added. It then shows in the Entity Properties and can be set."
    }
  ]
}
[/block]

To add variables in MBScript, use the '+' button or the 'Add' dropdown at the top and select 'Add Variable'. You then select the variable type.

Variable types that have a value (like Number, Text, 'Entity', 'Entity Asset') can have a Default Value set (which will be the starting value when the MBScript is added to a Entity).
[block:api-header]
{
  "title": "Variable Types"
}
[/block]
* Basic types like Bool (True/False), Number, Text
* All [Assets](doc:importing-assets) types, like Entity Assets, Materials, Audioclips, etc
* Vectors, Range (with a min / max number)
* Entity: for a Entity in the world

Some variable types are made from multiple other types. If ‘Entity Component of X type’ is selected, you then select the type of Entity Component. This could be a component on a Entity like Transform / Health System, or could be another MBScript

[block:api-header]
{
  "title": "Methods and ReturnMethods"
}
[/block]
Methods can be added that other scripts can call. They can have parameters set to pass values.

ReturnMethod are methods that return a value. 
[block:image]
{
  "images": [
    {
      "image": [
        "https://files.readme.io/f3490b8-ReturnMethods.PNG",
        "ReturnMethods.PNG",
        716,
        223,
        "#1f3f4c"
      ],
      "caption": "A 'Set to Red' method is given a Entity to set it's color to Red.\nA 'Is Entity Red' method returns True if the Entity is red."
    }
  ]
}
[/block]

[block:api-header]
{
  "title": "Event Variables"
}
[/block]
Added variables can also include new Events. Events can be called in the same script or in other entities.

Events are used to have any other MBScript code run when it's called - rather than just specific code like Methods.

If ‘Event(x)’ is selected, then an event variable with a parameter type is added (with the ‘x’ meaning you then select the parameter type). That way the Event can be called passing a value
[block:image]
{
  "images": [
    {
      "image": [
        "https://files.readme.io/7b42695-SawEntity.png",
        "SawEntity.png",
        762,
        353,
        "#163e4f"
      ],
      "caption": "Here every update it would call the 'Saw Entity' event for each Entity that was within 1m"
    }
  ]
}
[/block]


[block:api-header]
{
  "title": "Lists"
}
[/block]
When creating a variable type with a value there is a option to 'Create as List'.

If a variable is a List it'll show borders on the side of the icon.
[block:image]
{
  "images": [
    {
      "image": [
        "https://files.readme.io/08e611a-EntityList.png",
        "EntityList.png",
        1128,
        291,
        "#164052"
      ],
      "caption": "A 'List of entities' variable is added. And on start it's set to all entities within 1 meter.\nThen the 'Die' method is run on the first Entity in the list."
    }
  ]
}
[/block]

[block:api-header]
{
  "title": "PlayTime Variable"
}
[/block]
PlayTime variables store the current 'play mode time': seconds since play mode started.

Each PlayTime variable also has a event added for when it's 'Lapsed'. Which can be a useful way to run code after a set amount of time / on a specific time loop

[block:image]
{
  "images": [
    {
      "image": [
        "https://files.readme.io/c7745c1-NextSound.png",
        "NextSound.png",
        796,
        290,
        "#1a3947"
      ],
      "caption": "'Next Sound Effect' Play Time variable is added. The 'PlayAudio' method runs on Start, and when NextSoundEffect lapses - it then sets the 'NextSoundEffect' to the current time plus 3 seconds"
    }
  ]
}
[/block]