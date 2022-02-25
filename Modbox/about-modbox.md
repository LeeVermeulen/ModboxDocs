---
title: "About Modbox"
slug: "about-modbox"
hidden: false
createdAt: "2020-05-25T06:09:55.704Z"
updatedAt: "2021-06-14T15:23:56.059Z"
---
Modbox is a multiplayer game creation sandbox for PC / VR / AR - by [Alientrap](http://www.alientrap.com). Build and play games with other players online in real time. 
[block:callout]
{
  "type": "info",
  "title": "Modbox out now Steam",
  "body": "[http://store.steampowered.com/app/414120/](http://store.steampowered.com/app/414120/)\nAR version of Modbox is out now for [MagicLeap](doc:magicleap)"
}
[/block]

[block:embed]
{
  "html": "<iframe class=\"embedly-embed\" src=\"//cdn.embedly.com/widgets/media.html?src=https%3A%2F%2Fwww.youtube.com%2Fembed%2FKoRw38Dj1r0%3Ffeature%3Doembed&display_name=YouTube&url=https%3A%2F%2Fwww.youtube.com%2Fwatch%3Fv%3DKoRw38Dj1r0&image=https%3A%2F%2Fi.ytimg.com%2Fvi%2FKoRw38Dj1r0%2Fhqdefault.jpg&key=f2aa6fc3595946d0afc3d76cbbd25dc3&type=text%2Fhtml&schema=youtube\" width=\"854\" height=\"480\" scrolling=\"no\" title=\"YouTube embed\" frameborder=\"0\" allow=\"autoplay; fullscreen\" allowfullscreen=\"true\"></iframe>",
  "url": "https://www.youtube.com/watch?v=KoRw38Dj1r0",
  "title": "Modbox 2.0 - Game Creation Sandbox",
  "favicon": "https://www.youtube.com/s/desktop/75da313d/img/favicon.ico",
  "image": "https://i.ytimg.com/vi/KoRw38Dj1r0/hqdefault.jpg"
}
[/block]
## Multiplayer Creation
* Create Multiplayer / Singleplayer / Coop games while switching between VR and Desktop on PC. Or create games in your own environment on a AR device like MagicLeap. Everything is synced with other online players in real time.
* Share Creations made on Steam Workshop or on ModboxGame.com
* Use any of the editor tools while playing. There are both [Tools](doc:tools) used for hands / while playing as a avatar, and a [Desktop Editor](doc:desktop-editor) mode
* Play and edit with other players in **[Local Multiplayer](doc:local-multiplayer)** with up to 4 players locally with split screen (or Keyboard or Gamepads) with another player in VR. Local players can also play online.
* **[Prefabs](doc:prefabs)** can be used to create reusable parts out of Creations. Prefabs can then be shared online for other creators to use - and can include assets (3d models, visual scripting, C# projects). Prefabs can also include other nested prefabs, allow for easily building large complex worlds out of reusable parts.
* Create a server at anytime (while playing or editing), and use the ** [Servers Permissions](doc:server-settings)** system to control who can administer/ edit / play on your server.

## Advanced Scripting
* The ingame visual scripting system **[MBScript](doc:mbscript)** can be used for scripting gameplay / AI / Physics. MBScript is a drag and drop visual scripting system that has both a node like tool (using the **[Wiring](doc:wiring)** tool/desktop window), and a Blocks/Scratch like interface for more advanced building (using the same type system as C#). 
* MBScript can be edited both visually with drag and drop, and in the ingame text editor (with autocomplete using a ingame VisualStudioCode Monaco editor). MBScript can be used to create complex AI characters and multiplayer bots.
* The **[C# Compiler](doc:c-compiler)** mod (coming soon to PC platform only) allows for writing your own C# code to include in Creations. Can add new [Entity Components](doc:components-1), editor tools, or new functions and options to run in MBScript / Wiring. Open C# projects in VisualStudio, and write code while the game is running for instantly compiling and seeing changes. All the Modbox game and editor tool C# source is included as reference/editable ingame.

## Physics and Interaction
* Full body VR simulation and physics based VR locomotion. All game objects were designed first for VR interaction (including reloading clips into guns, pulling bows to fire arrows, etc), with procedural animation used for Desktop players / AI to do same actions.
* Physics and Destruction - Building physics creations in Modbox does not use a physics hierarchy like other level editors / game creations tools. Instead 'Connections' are made between physics objects when editing, which will join them together in play mode with physics. This allows for realistic destruction and dynamic environments.
* [Voxel Editing](doc:voxel-editing) allow for destruction and modifying while playing.

## Editing and Building
* Create UI interfaces with **[UI Entities](doc:building-ui)** - using the same visual scripting / wiring systems as world creation to create HUDs and other in world UI for players (including new Tools and Menus)
* Use the **[Voxel Editing](doc:voxel-editing)** tool and desktop window to create large voxel terrains, with caves / hills / buildings. Create smooth voxel worlds or switch to Cubic for Minecraft-style blocks.
* **[Mesh Editing](doc:mesh-editing)** tools for creating meshes out of primitives ingame

## Moddable
* **[Assets](doc:assets)** System with **[Importing Assets](doc:importing-assets)** - Import 3d models, humanoid models, textures, sounds. All at runtime while playing. Use the [Material Editor](doc:material-editor)  to set material properties. Import 3d models from online sources including Google Poly (SketchFab coming soon)
* Everything in Modbox is a mod - including default included mods like SteamVR / Oculus VR support, Steamworks, Nvidia Flex liquid/soft particles, and editor tools like [Mesh Editing](doc:mesh-editing) and [Voxel Editing](doc:voxel-editing). It's designed to be as extensible and configurable as possible.
* Mods can contain assets and be used in creations (such as the Modern Weapons mod) that players will download to play the creation. Or they can be <<glossary:Local Mod>>s, basically Plugins, adding options and features just to the local players
* Use the **[ModboxSDK](doc:modboxsdk-guide)** Unity package to create Modbox mods in the Unity Editor. Mods can include Unity scenes turned into [Environments](doc:environments), GameObjects/Prefabs into Entity Assets, avatars into [Humanoid Models](doc:humanoid-models). Mods can also include new editor tools built in C#.