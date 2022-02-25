---
title: "EntUser"
slug: "entuser"
hidden: false
createdAt: "2020-11-10T21:51:06.659Z"
updatedAt: "2021-06-18T01:38:07.680Z"
---
**User**
A Connected User (not their ingame Avatar)

ID: EntUser
Base Type: [Entity Component](doc:componententity)

[block:api-header]
{
  "title": "Values"
}
[/block]

[block:parameters]
{
  "data": {
    "h-0": "Name",
    "h-1": "Type",
    "h-2": "Description",
    "0-0": "Player Avatar",
    "0-1": "Entity Component Variable<Player Avatar>",
    "0-2": "The User's current Avatar in the World",
    "1-0": "Avatar Asset",
    "1-1": "Entity Asset With Component Variable<Player Avatar>",
    "1-2": "Player Avatar to Spawn",
    "2-0": "Set Avatar On Team",
    "2-1": "Team Variable",
    "2-2": "Sets the Team variable of the Team component on the PlayerAvatar, if it has one",
    "3-0": "Spawn Count",
    "3-1": "Int Variable",
    "3-2": "#",
    "4-0": "Score",
    "4-1": "Number Variable",
    "4-2": "#",
    "5-0": "Input Type",
    "5-1": "Enum Variable<MB Input Device Type>",
    "5-2": " - ReadOnly",
    "6-0": "Local User Num",
    "6-1": "Int Variable",
    "6-2": " - ReadOnly",
    "7-0": "User State",
    "7-1": "Enum Variable<User State>",
    "7-2": " - ReadOnly",
    "8-0": "In Hieachry Mode",
    "8-1": "Entity Variable",
    "8-2": " - ReadOnly",
    "9-0": "User Name",
    "9-1": "Text Variable",
    "9-2": "Defaults to Player",
    "10-0": "User Started Playing",
    "10-1": "Bool Variable",
    "10-2": "Set to True once the user is in Playing state and after UserStartedPlaymode event -  - ReadOnly"
  },
  "cols": 3,
  "rows": 11
}
[/block]

[block:api-header]
{
  "title": "Methods"
}
[/block]

[block:parameters]
{
  "data": {
    "h-0": "Name",
    "h-1": "Description",
    "0-0": "Can Use Player Avatar In World",
    "0-1": "Bool",
    "0-2": "Returns if a User can use a Avatar in the world. Will return false if Avatar is Disabled/In Edit mode - or if the avatar/user is VR and the user/avatar is not",
    "1-0": "Switch User State",
    "1-1": "",
    "1-2": "",
    "2-0": "Spawn Avatar()",
    "2-1": "Spawns Avatar at Spawn Spots or at the Start Height",
    "3-0": "Spawn Avatar At Position(Vector3 groundPosition, Vector3 spawnRotation)",
    "3-1": "Spawns Avatar at Position/Angle",
    "4-0": "Print Message(Text message)",
    "4-1": "Print a message just to this user",
    "5-0": "Show UI Screen(UI Screen canvasScreen)",
    "5-1": "Show a UI Screen asset to this user",
    "6-0": "Close UI Screen()",
    "6-1": "Close any UI Screen the user currently has open",
    "7-0": "Show Message In UI Screen(Text message)",
    "7-1": "Show a message as a UI Screen asset to this user"
  },
  "cols": 2,
  "rows": 8
}
[/block]

[block:api-header]
{
  "title": "Properties"
}
[/block]

[block:parameters]
{
  "data": {
    "h-0": "Name",
    "h-1": "Type",
    "h-2": "Description",
    "0-0": "Is VR User",
    "0-1": "Bool",
    "0-2": "",
    "1-0": "Is Screen User",
    "1-1": "Bool",
    "1-2": "",
    "2-0": "Is Local User",
    "2-1": "Bool",
    "2-2": "",
    "3-0": "Is Bot User",
    "3-1": "Bool",
    "3-2": "",
    "4-0": "Appearence Info",
    "4-1": "Text",
    "4-2": "",
    "5-0": "Client",
    "5-1": "Client",
    "5-2": ""
  },
  "cols": 3,
  "rows": 6
}
[/block]


Attributes:
ModboxMain.MBTypeComponentNoIngameAddingAttribute
ModboxMain.MBTypeComponentEnabledInEditmodeAttribute
ModboxMain.MBOldIDAttribute