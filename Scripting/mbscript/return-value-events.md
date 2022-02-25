---
title: "Return Value Events"
slug: "return-value-events"
hidden: false
createdAt: "2021-06-17T20:01:45.228Z"
updatedAt: "2021-06-17T20:55:19.934Z"
---
* Some Components will have a 'Return Value Event' so that other components/MBScript can return a Value when a event happens.
[block:image]
{
  "images": [
    {
      "image": [
        "https://files.readme.io/81c5917-DamageModifer.PNG",
        "DamageModifer.PNG",
        770,
        336,
        "#1a3947"
      ],
      "caption": "The 'Health System Damage Modifer' component has a 'Ignore Damage' return value event. This script returns 'True' if the damage is less than 10.\n\nThis script can also modify the damage done -  setting it to 10 if the damage is from a Toy"
    }
  ]
}
[/block]
* Code running inside a 'Return Value Event' can't change values on the Entity or World, or do operations. The reason for this is so the Return Value can be run at any time (like on hovering over the variable or viewing it in Entity Properties) and not have unexpected [side effects](https://en.wikipedia.org/wiki/Side_effect_%28computer_science%29).
* ReturnValue Events always run Locally for Players - rather than running just on the server by default like normal MBScript events.

* Multiple Event lines can be added with the same 'Return Value' variable.  The *first* 'ReturnValue' line will set the value (the order of event lines can be set with [MBScript Attributes](doc:mbscript-attributes) )
[block:api-header]
{
  "title": "Creating Return Value Event"
}
[/block]
Use ‘ReturnValue>x’, to create an Event that returns a value. This can also have parameters (if ReturnEvent(y)>x is selected).
[block:image]
{
  "images": [
    {
      "image": [
        "https://files.readme.io/0eec8c3-0a03ba3-ReturnValueEvent.png",
        "0a03ba3-ReturnValueEvent.png",
        447,
        352,
        "#193b4c"
      ],
      "caption": "The 'Can Pickup Weapon' is a ReturnValue event. Here 'Can Pickup Weapon' is True if the entity has a Health System.\nThe HealthSystem is shown as greyed out, since this Entity doesnt have it yet."
    }
  ]
}
[/block]

[block:image]
{
  "images": [
    {
      "image": [
        "https://files.readme.io/5fd4f02-2fcdaf3-ReturnValue.png",
        "2fcdaf3-ReturnValue.png",
        787,
        333,
        "#193947"
      ],
      "caption": "A 'Get Move Speed For Player' ReturnValue variable is added, with a parameter type of 'Player'. This sets it's Movement Speed to '30' only if it's on the Enemy team - otherwise it'll have it's default value of 100.\n\nAnother script could also then add a Event line to return a value."
    }
  ]
}
[/block]