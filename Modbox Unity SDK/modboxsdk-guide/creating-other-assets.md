---
title: "Creating Other Assets"
slug: "creating-other-assets"
hidden: false
createdAt: "2020-05-25T05:23:21.249Z"
updatedAt: "2020-08-27T15:08:15.519Z"
---
[Unity Scenes to Environment Assets](doc:unity-scenes-to-environment-assets) 

[Humanoid Models](doc:humanoid-models) - Create <<glossary:Humanoid Model>> from Unity Humanoid models

[Materials](doc:material-editor) Assets - A Material asset sets the Unity Material to the game object's mesh renderers - and also sets the ModboxPhysicsMaterial. Use  'Create Modbox Material' to create one after selecting a Unity Material in the project view. Use 'Auto Create Icons' option in MBEngine to create the icon for the material ingame.

##New Prefabs
For creating new Big UI Screens, Ent Modifiers, Desktop Windows, VR Tools - the easiest way is to duplicate a existing prefab of that type (some found in Resources/Mods/Main/') then move that prefab to your mods directory. You then need to create a 'Asset' that points to this prefab, which can be done by right clicking and selecting 'Create Asset For Mod Prefab'

##Audio Clip
Audio Clip assets can be selected in Modbox to add as sound effects / music ingame. Right click on a AudioClip file and select 'Create Modbox Audio Clip'

##Physics Material
Use  'Create Modbox Physics Material' to create one after selecting a Unity Physics Material in the project view. A 'Modbox Physics Material' sets the physics material for a material, or entity, and has settings for sound / break force.

##Font
'Create Modbox Font' when selecting a font asset in the project view.