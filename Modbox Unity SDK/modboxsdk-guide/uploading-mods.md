---
title: "Uploading Mods"
slug: "uploading-mods"
hidden: false
createdAt: "2020-05-25T05:28:26.659Z"
updatedAt: "2021-07-03T21:47:12.243Z"
---
Modbox Mods are built as multiple Unity Asset Bundles - 1 asset bundle to hold the mod info and other information (like icons), 1 for all the assets, and 1 for the scenes.

Usually when testing mods in the Unity editor they will be loaded as '**Simulated Mods**'. This will load the entities/content directly from the mod directory rather than asset bundles - so you can make quick changes and not have to rebuild the asset bundles each time.

## Uploading a Mod to the Workshop
In the Mod asset, use the 'Build and Publish Mod' button. This will first build the asset bundles and put them in the Streaming Assets folder.
By default all content in the mod directory is added to the asset bundle. If your building a lot of content you will want to put all non entities not using in a 'BuildIgnore' directory, or add a ignore directory name in the 'Ignore Directories' list. When creating asset bundles Unity will add in all needed content that the Entities use.
 
To test a built mod, use 'Load Built Mods First' in the 'MBStartUp' gameobject.