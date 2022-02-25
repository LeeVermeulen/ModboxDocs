---
title: "Server"
slug: "server"
hidden: false
createdAt: "2020-11-06T00:58:26.884Z"
updatedAt: "2021-07-11T14:08:58.535Z"
---
Current Server all connected clients are in


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
    "0-0": "Mods: Enabled Server Mods",
    "0-1": "Mod Info Variable List",
    "0-2": "All Server mods Enabled -  - ReadOnly",
    "1-0": "Server Settings: Room Code",
    "1-1": "Text Variable",
    "1-2": "Defaults to  -  - ReadOnly",
    "2-0": "Server Settings: Public Listed",
    "2-1": "Bool Variable",
    "2-2": "Sets if this server will show in public server listings to join. Otherwise players have to enter Room Code - Defaults to True",
    "3-0": "Server Settings: Set Password",
    "3-1": "Bool Variable",
    "3-2": "",
    "4-0": "Server Settings: Password",
    "4-1": "Text Variable",
    "4-2": "",
    "5-0": "Server Settings: Max Players",
    "5-1": "Int Variable",
    "5-2": "Defaults to 8 - #",
    "6-0": "Server Settings: Default Role",
    "6-1": "Enum Variable<MB Role>",
    "6-2": "Set default role for anyone joining server. Their Role sets their permissions for what they can control / play - Defaults to CanEdit",
    "7-0": "Server Settings: Network Mode",
    "7-1": "Network Mode Variable",
    "7-2": "",
    "8-0": "Server Settings: Voice Chat",
    "8-1": "Bool Variable",
    "8-2": "Defaults to True",
    "9-0": "Server Settings: Positional Voice Chat",
    "9-1": "Bool Variable",
    "9-2": "Defaults to True",
    "10-0": "Server Settings: Quick Roll Off",
    "10-1": "Bool Variable",
    "10-2": "Voice audio will 'roll off' logarithmic rather than linear so only nearby users can hear",
    "11-0": "Server Settings: Switch Hosts On Disconnect",
    "11-1": "Bool Variable",
    "11-2": "Host will switch to another player if the Host disconnects - Defaults to True",
    "12-0": "Server Settings: Sync Asset Files",
    "12-1": "Bool Variable",
    "12-2": "Host and clients will send Asset files to other clients for imported content (Only if they have Edit Permission to import content) - Defaults to True",
    "13-0": "Server Settings: Strict Permissions",
    "13-1": "Bool Variable",
    "13-2": "Will stop users from changing Entities they dont have permission to edit based on their Role - and give them a error message on trying",
    "14-0": "Server Settings: Server Name",
    "14-1": "Text Variable",
    "14-2": "Set a name to display in Listings",
    "15-0": "Server Settings: Server Description",
    "15-1": "Text Variable",
    "15-2": "Set a description to display in Listings"
  },
  "cols": 3,
  "rows": 16
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
    "0-0": "State: Switch To Play Mode(Bool testmode)",
    "0-1": "",
    "1-0": "State: Switch To Edit Mode()",
    "1-1": "",
    "2-0": "State: Reset Playmode()",
    "2-1": "",
    "3-0": "State: Switch Creation(Creation Meta Data creation, Bool playmode)",
    "3-1": "",
    "4-0": "State: Switch To Lobby()",
    "4-1": "",
    "5-0": "Server System: Show Message Server(Text textToShow)",
    "5-1": "",
    "6-0": "Server System: User Chat(Text textToShow)",
    "6-1": "",
    "7-0": "Server System: Kick Client(Client client)",
    "7-1": "",
    "8-0": "Server System: Ban Client(Client client)",
    "8-1": "",
    "9-0": "Server System: Change Client Role(Client client, MB Role newRole)",
    "9-1": ""
  },
  "cols": 2,
  "rows": 10
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
    "0-0": "Clients: Is Master Client",
    "0-1": "Bool",
    "0-2": "Returns True if the local system is Master Client",
    "1-0": "Clients: Local Client",
    "1-1": "Client",
    "1-2": "",
    "2-0": "Clients: Master Client",
    "2-1": "Client",
    "2-2": "",
    "3-0": "Clients: All Clients",
    "3-1": "Client List",
    "3-2": "",
    "4-0": "Server Settings: Net Status Text",
    "4-1": "Text",
    "4-2": "",
    "5-0": "Server Settings: Network Description Text",
    "5-1": "Text",
    "5-2": ""
  },
  "cols": 3,
  "rows": 6
}
[/block]