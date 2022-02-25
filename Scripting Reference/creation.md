---
title: "Creation"
slug: "creation"
hidden: false
createdAt: "2021-06-18T01:50:04.782Z"
updatedAt: "2021-07-11T14:08:58.549Z"
---
The current <<glossary:Creation>> loaded


[block:api-header]
{
  "title": "Create"
}
[/block]

[block:parameters]
{
  "data": {
    "h-0": "Name",
    "h-1": "Type",
    "h-2": "Description",
    "0-0": "Assets: Rename Asset(Mod Asset asset, Text newName, Bool keepOldName)",
    "0-1": "Mod Asset",
    "0-2": "",
    "1-0": "Assets: Create New Asset(MB Type Mod Asset assetType, Text name, Mod Location location)",
    "1-1": "Mod Asset",
    "1-2": "",
    "2-0": "Assets: Clone Asset(Mod Asset clonedAsset, Text newName)",
    "2-1": "Mod Asset",
    "2-2": "",
    "3-0": "Prefabs: Create New Prefab From Entity(Entity worldEnt, Text prefabName)",
    "3-1": "Entity MB Prefab Creation",
    "3-2": "",
    "4-0": "Prefabs: Create New Prefab Group With Entities(Entity List entities, Text prefabName)",
    "4-1": "Entity",
    "4-2": ""
  },
  "cols": 3,
  "rows": 5
}
[/block]

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
    "0-0": "Metadata: Creation Name",
    "0-1": "Text Variable",
    "0-2": "",
    "1-0": "Metadata: Creation Description",
    "1-1": "Text Variable",
    "1-2": "",
    "2-0": "Metadata: Creation Tags",
    "2-1": "Text Variable List",
    "2-2": "",
    "3-0": "Metadata: In Development",
    "3-1": "Bool Variable",
    "3-2": "Will tell players this creation is still in development",
    "4-0": "Metadata: Multiplayer Only",
    "4-1": "Bool Variable",
    "4-2": "If this creation requires multiple players to play properly",
    "5-0": "Metadata: VR Player Required",
    "5-1": "Bool Variable",
    "5-2": "If this creation requires a VR player to play properly",
    "6-0": "Metadata: Screen Player Required",
    "6-1": "Bool Variable",
    "6-2": "If this creation requires a Screen Player to play properly",
    "7-0": "Metadata: Creator Account Required",
    "7-1": "Bool Variable",
    "7-2": "If this creation uses online services/mods that use a Modbox creator account (Voice/AI)",
    "8-0": "Misc: Creation Color Palette",
    "8-1": "Color Variable List",
    "8-2": "",
    "9-0": "Players: Allow Playmode Editing",
    "9-1": "Bool Variable",
    "9-2": "Allows player avatars to use editing tools while playing - Defaults to True",
    "10-0": "Players: Playmode Test Mode",
    "10-1": "Bool Variable",
    "10-2": "Set to True on running the creation in Test mode. Users wont switch to Playing state on start -  - ReadOnly",
    "11-0": "Players: Pause In Menu",
    "11-1": "Bool Variable",
    "11-2": "Will pause the world when the menu is being used when not online - Defaults to True",
    "12-0": "VR: Force Locomotion",
    "12-1": "Locomotion Variable",
    "12-2": "If set, will override the VR Players locomotion",
    "13-0": "VR: Set VR Speed",
    "13-1": "Bool Variable",
    "13-2": "Set a move speed for all VR players",
    "14-0": "VR: Set VR Move Speed",
    "14-1": "Number Variable",
    "14-2": "Defaults to 3 - m/s",
    "15-0": "VR: Limit VR Speed",
    "15-1": "Bool Variable",
    "15-2": "Limit VR Move speed to a maximum",
    "16-0": "VR: VR Speed Limit",
    "16-1": "Number Variable",
    "16-2": "Defaults to 3 - m/s",
    "17-0": "VR: No Teleporting",
    "17-1": "Bool Variable",
    "17-2": "",
    "18-0": "VR: No Air Control",
    "18-1": "Bool Variable",
    "18-2": "",
    "19-0": "VR: Show Pickup Tool",
    "19-1": "Bool Variable",
    "19-2": "Defaults to True",
    "20-0": "Worlds: Current World",
    "20-1": "World Variable",
    "20-2": "",
    "21-0": "Worlds: Start World",
    "21-1": "World Variable",
    "21-2": "",
    "22-0": "Misc: Log Error On Operations",
    "22-1": "Bool Variable",
    "22-2": "Will log User error when running Do/Set lines and variable is not found - Defaults to True",
    "23-0": "Misc: MB Script Debug Mode",
    "23-1": "Bool Variable",
    "23-2": "User Errors will be shown on the UI, and will pause on any set Breakpoints.",
    "24-0": "Misc: MB Script Breakpoint On Error",
    "24-1": "Bool Variable",
    "24-2": "Will Pause game and focus on Breakpoint on a Error",
    "25-0": "Mods: Load All Mod Assets",
    "25-1": "Bool Variable",
    "25-2": "By default when Play mode is started only assets that are used are loaded - use this to load all of them",
    "26-0": "Mods: Load All Assets From Mods",
    "26-1": "Mod Variable List",
    "26-2": "By default when Play mode is started only assets that are used are loaded - use this to load all assets from certain mods",
    "27-0": "Mods: Enabled Creation Mods",
    "27-1": "Mod Info Variable List",
    "27-2": "Data on all mods enabled in Creation -  - ReadOnly",
    "28-0": "Audio: Player Died Sound",
    "28-1": "Audioclip Variable",
    "28-2": "",
    "29-0": "Audio: Other Player Died Sound",
    "29-1": "Audioclip Variable",
    "29-2": "",
    "30-0": "Game: Unlimited Ammo",
    "30-1": "Bool Variable",
    "30-2": "",
    "31-0": "Game: No Player Damage",
    "31-1": "Bool Variable",
    "31-2": "No damage to any players - 'God Mode'",
    "32-0": "Game: No Friendly Fire",
    "32-1": "Bool Variable",
    "32-2": "No damage from Entities on same Team",
    "33-0": "Game: No Grab Outline",
    "33-1": "Bool Variable",
    "33-2": "No outline will be shown on grabbing items",
    "34-0": "Game: No Toy Handle Highlight",
    "34-1": "Bool Variable",
    "34-2": "Toy handles won't be highlighted",
    "35-0": "Players: Users Can Spawn",
    "35-1": "Bool Variable",
    "35-2": "Users can Spawn themselves - Defaults to True",
    "36-0": "Players: Users Spawn At Start",
    "36-1": "Bool Variable",
    "36-2": "Users will try spawning themselves on switching to Playing state - Defaults to True",
    "37-0": "Players: Default Avatar",
    "37-1": "Entity Asset With Component Variable<Player Avatar>",
    "37-2": "The default avatar asset to use for users",
    "38-0": "Players: Default Avatar VR",
    "38-1": "Entity Asset With Component Variable<Player Avatar>",
    "38-2": "The default avatar asset to use for VR users. Will use the default avatar asset if not set",
    "39-0": "Players: Game Menu",
    "39-1": "UI Screen Entity Canvas Variable",
    "39-2": "A UI Screen to use as the creation's Menu. Will show as a button option to open for Screen+VR users",
    "40-0": "Players: Add Components To Users",
    "40-1": "MB Script Entity Component Type Variable List",
    "40-2": "Will add MBScript components to users on starting Play mode",
    "41-0": "Players: Add Name Tags To Player Avatars",
    "41-1": "Bool Variable",
    "41-2": "Defaults to True",
    "42-0": "Players: Allow Flying",
    "42-1": "Bool Variable",
    "42-2": "",
    "43-0": "Players: Climb All Static",
    "43-1": "Bool Variable",
    "43-2": "Allow climbing anything static, not just climbable parts. VR Players only currently.",
    "44-0": "Players: Remove Avatar On User Left",
    "44-1": "Bool Variable",
    "44-2": "When a user leaves a avatar (exits game / changes mode) remove the avatar - Defaults to True",
    "45-0": "Metadata: Save Internal",
    "45-1": "Bool Variable",
    "45-2": "",
    "46-0": "Metadata: Save Template",
    "46-1": "Bool Variable",
    "46-2": "",
    "47-0": "Metadata: Template Order",
    "47-1": "Number Variable",
    "47-2": "",
    "48-0": "Metadata: Save Included",
    "48-1": "Bool Variable",
    "48-2": "",
    "49-0": "Players: Default HUD",
    "49-1": "Entity Asset With Component Variable<UI Canvas>",
    "49-2": "Default UI Canvas to set as the Player Avatar's HUD. Can be overridden on the User/Avatar"
  },
  "cols": 3,
  "rows": 50
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
    "0-0": "Assets: Delete Asset(Mod Asset asset)",
    "0-1": "",
    "1-0": "Assets: Rename Asset(Mod Asset asset, Text newName, Bool keepOldName)",
    "1-1": "",
    "2-0": "Assets: Create New Asset(MB Type Mod Asset assetType, Text name, Mod Location location)",
    "2-1": "",
    "3-0": "Assets: Clone Asset(Mod Asset clonedAsset, Text newName)",
    "3-1": "",
    "4-0": "Assets: Sync Asset Files(Byte List fileData, Mod Asset asset)",
    "4-1": "",
    "5-0": "Prefabs: Create New Prefab From Entity(Entity worldEnt, Text prefabName)",
    "5-1": "",
    "6-0": "Prefabs: Create New Prefab Group With Entities(Entity List entities, Text prefabName)",
    "6-1": "",
    "7-0": "Prefabs: Remove Prefab Data(Entity ent)",
    "7-1": "",
    "8-0": "Prefabs: Remove Prefab And Delete Instances(Entity MB Prefab Creation prefabAsset)",
    "8-1": "",
    "9-0": "Prefabs: Remove Prefab And Un Prefab Instances(Entity MB Prefab Creation prefabAsset)",
    "9-1": "",
    "10-0": "Worlds: Create New World(MB Widget Button)",
    "10-1": "",
    "10-2": "",
    "11-0": "Worlds: Reload World()",
    "11-1": "",
    "12-0": "Mods: Enable Mod(Modbox Mod mod)",
    "12-1": "",
    "13-0": "Mods: Disable Mod(Modbox Mod mod)",
    "13-1": ""
  },
  "cols": 2,
  "rows": 14
}
[/block]

[block:api-header]
{
  "title": "Events"
}
[/block]

[block:parameters]
{
  "data": {
    "h-0": "Name",
    "h-1": "Description",
    "0-0": "Players: Creation Playmode Started()",
    "0-1": "Runs when Playmode first starts in the Creation"
  },
  "cols": 2,
  "rows": 1
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
    "0-0": "Assets: Clone Asset Called(Mod Asset, Text)",
    "0-1": "Mod Asset",
    "0-2": "",
    "1-0": "Assets: Create New Asset Called(MB Type Mod Asset, Text, Mod Location)",
    "1-1": "Mod Asset",
    "1-2": "",
    "2-0": "Players: Playmode Time",
    "2-1": "Number",
    "2-2": "Time since start of the Creation's play mode",
    "3-0": "Assets: All Enabled Mods",
    "3-1": "Modbox Mod List",
    "3-2": "",
    "4-0": "Assets: Loaded Assets From Mod(Modbox Mod)",
    "4-1": "Mod Asset List",
    "4-2": "",
    "5-0": "Assets: Loaded Assets Of Type(MB Type Mod Asset)",
    "5-1": "Mod Asset List",
    "5-2": "",
    "6-0": "Assets: Loaded Assets Of Type With Tag(MB Type Mod Asset, Tag In Asset)",
    "6-1": "Mod Asset List",
    "6-2": "",
    "7-0": "Assets: Loaded Entity Assets With Tag(Tag In Entity)",
    "7-1": "Entity Asset List",
    "7-2": "",
    "8-0": "Assets: Loaded Entity Assets With Component(MB Type Entity Component)",
    "8-1": "Entity Asset List",
    "8-2": "",
    "9-0": "Assets: Loaded Entity Assets",
    "9-1": "Entity Asset List",
    "9-2": "",
    "10-0": "Assets: Loaded Materials",
    "10-1": "Material List",
    "10-2": "",
    "11-0": "Assets: Loaded Humanoid Models",
    "11-1": "Humanoid Model List",
    "11-2": ""
  },
  "cols": 3,
  "rows": 12
}
[/block]