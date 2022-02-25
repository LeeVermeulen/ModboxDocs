---
title: "Creating a Mod"
slug: "creating-a-mod"
hidden: false
createdAt: "2020-05-25T05:23:21.566Z"
updatedAt: "2021-07-03T21:45:24.890Z"
---
Use the 'Create New Mod' option in the /Modbox menu. Set a unique mod name (something that won't be shared by other mods online). A new folder will be created for your mod, and a 'modmetadata' file to set your mod settings.

Put all your mod assets in this folder.

Back up your mod data! Preferably with a version control system - as Steam might wipe it out when updating the SDK

Mod Options:

* ModName - The 'ModName' is the name that is saved in creations - so it must be unique and not change.
* ModFullName - Full name displayed to the user.
* Description - shown on workshop page
* Icon - image for workshop page
* Published File ID: Workshop ID. Created on first upload to the workshop.
When you run the ModboxSDK in the Unity Editor your mod should now show in the 'mods' options ingame.