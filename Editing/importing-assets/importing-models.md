---
title: "Importing Models"
slug: "importing-models"
hidden: false
createdAt: "2020-11-06T15:18:38.302Z"
updatedAt: "2021-02-01T17:01:02.637Z"
---
[block:api-header]
{
  "title": "Importing FBX / GLTX / Obj models at Runtime"
}
[/block]
- To import models at Runtime (rather than built in the Unity SDK) - Modbox uses Trilib2: https://ricardoreis.net/trilib-2/
- A list of supported model formats can be found here: https://ricardoreis.net/accepted-file-formats/
- To test if your model should work in Modbox, there is a online web model viewer: https://ricardoreis.net/trilib/trilib2demo/modelviewer/
[block:api-header]
{
  "title": "Trilib: Importing Humanoid Models at Runtime"
}
[/block]
Can test avatars in the web importer here: https://ricardoreis.net/trilib/trilib2demo/avatarloader/

Follow directions here: [https://ricardoreis.net/avatar-importing/](https://ricardoreis.net/avatar-importing/) 
TriLib comes with the Mixamo and Biped Humanoid Avatar Mapper, which contains the settings to load characters rigged in Mixamo or created using 3Ds Max Biped, among other common bone hierarchies.

-It is important that your model is in T-Pose or Star-Pose.

Only FBX and GLTF file formats work as Avatars.

You can easily include your own bone-mapping schemes by inheriting the ByNameHumanoidAvatarMapper class or simply creating an instance from the class on your Assets and adding the name-mapping manually.

Here is a sample with all bone names accepted by the Mixamo and Biped Humanoid Avatar Mapper:

[block:image]
{
  "images": [
    {
      "image": [
        "https://files.readme.io/5a19409-bones.png",
        "bones.png",
        1100,
        650,
        "#141514"
      ]
    }
  ]
}
[/block]