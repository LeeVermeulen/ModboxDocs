---
title: "Modbox Unity SDK Guide"
slug: "modboxsdk-guide"
hidden: false
createdAt: "2020-05-25T13:26:07.950Z"
updatedAt: "2021-08-22T13:57:56.598Z"
---
ModboxSDK is a Unity Project for creating Modbox mods. It includes ways to create Modbox entities / humanoid models and other assets out of Unity Prefabs, and Environments from Unity scenes.

It can also be used as a way to debug and profile Creations (using the Unity debugger / profiler)

## Installing ModboxSDK
* The Modbox SDK is included as a zip file with the game's download on Steam. To find it: Right click on Modbox in the Steam Library and go into Properties->Local Files=>Browse
* Extract the ModboxSDK zip to your Desktop / anywhere outside of the Steam folder. If upgrading the SDK, extract  to a new folder (don't override old SDK folder)

## * Use Unity version: **2019.4.18** - Can be found here: https://unity3d.com/get-unity/download/archive.

[block:html]
{
  "html": "<h1><a href=\"unityhub://2019.4.18f1/3310a4d4f880\">Unity Hub Link to 2019.4.18</a></h1>"
}
[/block]

## Open the ModboxSDK folder as a Unity project (don't import it into a new/current project)


Video
[block:embed]
{
  "html": "<iframe class=\"embedly-embed\" src=\"//cdn.embedly.com/widgets/media.html?src=https%3A%2F%2Fwww.youtube.com%2Fembed%2FoLRWAiCJggU&display_name=YouTube&url=https%3A%2F%2Fwww.youtube.com%2Fwatch%3Fv%3DoLRWAiCJggU&image=http%3A%2F%2Fi.ytimg.com%2Fvi%2FoLRWAiCJggU%2Fhqdefault.jpg&key=f2aa6fc3595946d0afc3d76cbbd25dc3&type=text%2Fhtml&schema=youtube\" width=\"854\" height=\"480\" scrolling=\"no\" title=\"YouTube embed\" frameborder=\"0\" allow=\"autoplay; fullscreen\" allowfullscreen=\"true\"></iframe>",
  "url": "https://www.youtube.com/watch?v=oLRWAiCJggU",
  "title": "Modbox Unity SDK - Intro",
  "favicon": "https://www.youtube.com/s/desktop/9d8f3d46/img/favicon.ico",
  "image": "http://i.ytimg.com/vi/oLRWAiCJggU/hqdefault.jpg"
}
[/block]
## Trying out SDK
In the 'Modbox' folder, open the 'TestScene'. This is a testing blank scene for testing entities/creations. You should now be able to run the game and play Modbox in Unity.

## MBStartUp
The '**MBStartUp**' game object are settings for how to run the scene - highlight over the options for tool tips. Some options:
**Viewmode**: To set the game to start in VR, desktop, or VR Test, and AR options. See [Testing](doc:testing)  for the VR Testing controls

## Playing SDK - Asset Bundles
You can still load Modbox mods with the ModboxSDK - you just need to set the path to your Modbox mod directory to load the default mods that come with Modbox. Use the 'Modbox/SDK Settings' menu to set the right path.

By default mods will be loaded as 'Simulated' from the assets folder. Their prefabs are loaded directly - so changes that are made are made instantly.
You can turn this off and have the ModboxSDK load built mods first - with the 'Build Mods First' option in MBStartUp