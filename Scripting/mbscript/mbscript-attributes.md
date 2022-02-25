---
title: "MBScript Attributes"
slug: "mbscript-attributes"
hidden: false
createdAt: "2021-06-17T20:03:41.568Z"
updatedAt: "2021-06-17T21:16:40.572Z"
---
'Attributes' can be added to Variables or Event Lines to change some of their settings. Right click or click on the Keyword to then 'Add Attribute'
[block:api-header]
{
  "title": "Event Line Attributes"
}
[/block]

[block:image]
{
  "images": [
    {
      "image": [
        "https://files.readme.io/f35faf1-EventLineAttributes.PNG",
        "EventLineAttributes.PNG",
        622,
        341,
        "#0e6988"
      ],
      "caption": ""
    }
  ]
}
[/block]
Attributes can be added to Event Lines to set when they run (the order, or if they run locally/online) - hover over the ? to see their description.

By default MBScript code runs on the server - and sends all changed values/methods to all other online players.

This is usually how most code should run - but often you'd want code to run 'locally' so it's more responsive to players (like to play a 'Damage' effect immediately on a physics collision, rather than waiting 100ms for server to play Effect).

'Run On Controlled By' can be used to have MBScript only run on whatever client is 'controlling' the Entity - it'll then send all changed values to other clients. This can be useful for having responsive feedback to the player's actions. Players always 'Control' their own Avatars and whatever they are holding - then often will Control other entities in the world when they collide with them.

If 'Run Locally' is used - the MBScript will run on all clients and no changes will be sent online. This should be used to just show effects / feedback, since it might result in it happening only on some clients (if 'Run Locally' is used on a physics collision event it's possible that only 1 client had that physics collision happen).


Other Attribute options:
* 'Run In Editmode' can be used to have event lines run while editing
* Order can be set so that some MBScript Event Lines run before/after others that are linked to the same event.
* 'Immediate' will force the MBScript code to run immediately and not a frame later (MBScript code can often be delayed a frame)

[block:api-header]
{
  "title": "Value Attributes"
}
[/block]

[block:image]
{
  "images": [
    {
      "image": [
        "https://files.readme.io/2af2207-ValueAttributes.PNG",
        "ValueAttributes.PNG",
        608,
        390,
        "#125d79"
      ],
      "caption": "There are a number of Attribute options for value variables depending on the type - hover over the ? to see their description.\n\n'ReadOnly' will set the variable to only be edited inside this script."
    }
  ]
}
[/block]