---
title: "Unity Scenes to Environment Assets"
slug: "unity-scenes-to-environment-assets"
hidden: false
createdAt: "2020-05-26T06:47:53.219Z"
updatedAt: "2020-05-26T16:52:34.442Z"
---
Create a Environment Option asset in the right click menu in the Project view.

Environment options can be setup to just have a Skybox and ground settings (in which case the 'Env_Blank' Unity scene will be loaded, and those options set on it). Or they can be setup to load your own custom Unity scene.

## Setting up a Unity scene for Modbox
See example Environments in the Mods/Basics/Environments
Add the script '**MBEnvironmentSceneOptions**'. Adjust the Environment size so it contains your level (environment size is used for stuff like AI calculation, spatial positioning optimization, etc)
The bottom of the level should be at the zero Y position, and the the scene should be centered X/Z preferably
At any time just run Play to test the scene - it'll create a MBStartUp game object and start the game. If you want to run in a different view mode (like VR or VR Test), add a gameobject with the MBStartup script and you can set start settings in there.
Any game object in the scene that is just set to the Default layer will have it's layer changed to 'Environment'. The 'Environment' layer is used so entities are static when autoconnecting to it, teleporting ray in edit mode will collide with it, and AI will navigate on it.

## Sky Options
Add the 'MBEnvironmentSkybox' script to allow changing the skybox of the scene. A 'ModboxSkyPrefab' gameobject should be in a under this gameobject. The 'ModboxSkyPrefab' can be a Skybox prefab already made, or just a blank one

If the sky has a sun light, or a main light source (usually a directional light), place this in the ModboxSkyPrefab game object. This is so it'll be removed when the sky is changed.