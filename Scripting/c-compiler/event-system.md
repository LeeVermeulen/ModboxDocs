---
title: "Event System"
slug: "event-system"
hidden: false
createdAt: "2020-05-25T05:28:15.343Z"
updatedAt: "2020-10-31T16:23:56.731Z"
---
MBEvents are like C# delegates - but with a lot more options for ordering multiple actions, profiling, debugging, hooking into, and less error prone (no need to remove listeners of destroyed gameobjects/scripts). It doesn't replace the Unity Event system - it's more for broadcasting messages and allowing other gameobjects/systems to override easily, so that Modbox is easily moddable.

Use 'AddListener' on the event to subscribe to it.  All entities have events, and [MBVariables](doc:mbvariables) values have 'OnValueChanged' event that can be added to.

You do not need to run 'RemoveListener' when destroying the gameobject or removing the script. Methods on scripts/gameobjects that were removed won't be run (and will be removed from the event target list next time it's run). RemoveListener can be used to remove listeners before being destroyed though.


Examples of creating / responding to events:
[block:code]
{
  "codes": [
    {
      "code": "public MBEvent Event_GamePaused { get; } = new MBEvent ();\n\npublic MBEvent<ModboxClient> Event_ClientJoined { get; } = new MBEvent<ModboxClient>();\n\npublic MBEventReturn<Vector3, bool> Event_CanTeleport { get; } = new MBEventReturn<Vector3, bool>(true);\n\n// Then to add Listeners:\nprotected override void Awake()\n{\n  base.Awake();\n  Event_GamePaused.AddListener(OnEvent_GamePaused);\n  Event_ClientJoined.AddListener(OnEvent_ClientJoined);\n  Event_CanTeleport.AddListener(OnEvent_CanTeleport);\n}\n\nvoid OnEvent_GamePaused()\n{\n  // game paused...\n}\n\nvoid OnEvent_ClientJoined(ModboxClient Client)\n{\n  // new client...\n}\n\nbool CanTeleport(Vector3 Position)\n{\n  if (Position.y > 0)\n    return true;\n  else\n    return false;\n}\n",
      "language": "csharp"
    }
  ]
}
[/block]
ClientJoined is a example of a event with a single parameter (can have up to 6 parameters)

For naming convention, try to use 'Event_' for the event variables, and 'OnEvent_' for the method.

When using 'AddListener' you can set if the order the method should run compared to other methods.\

Events will still run if a script is disabled - but will not run if it's on a inactive game object (unless 'RunWhenDisabled' AddListener arguement is set to True )

You can always use AddListener to add a parameterless Action to any event (even if that Event has parameters). When adding a parameterless Action you can use 'AddNextUpdateListener' to have the method called the next update. This can be useful for avoiding running a method multiple times per frame and only wanting to update once (like update the UI).

## MBEventReturn
MBEventReturn can return values:
[block:code]
{
  "codes": [
    {
      "code": "public MBEventReturn<Vector3, bool> Event_CanTeleport { get; } = new MBEventReturn<Vector3, bool>(true);       \n\nbool CanTeleport(Vector3 Position)\n{\n        if (Position.y > 0)\n                return true;\n        else\n                return false;\n}\n\nvoid Update()\n{\n        if (Event_CanTeleport.Run())\n            Debug.Log(\"Can teleport!\");\n}",
      "language": "text"
    }
  ]
}
[/block]
'CanTeleport' is a example of a event with a return value. When the event is run, it will return the first non-default value (the default value is set when creating the event). So it will keep checking Listeners for the CanTeleport until False is returned. This is a great way to have a event run that other code can hook into and set. For example there could be a TeleportBlocker gameobject that listens for the CanTeleport event, and returns False if the position is inside it's bounds.