---
title: "Voxel Editing"
slug: "voxel-editing"
hidden: false
createdAt: "2020-05-25T06:35:55.281Z"
updatedAt: "2020-05-26T03:44:24.280Z"
---
* Use the Voxel Sculpter Tool or Desktop Window to sculpt voxel terrain
* Voxel terrain can have different resolutions and environment sizes. Use the 'Generate New' to change the environment size / voxel resolution.
* Switch between different voxel editing modes: Sculpt (sculpt with a cursor on the mouse / controller and set it's distance), Surface (sculpt on the first surface pointed at by mouse / controller), Block (Create a block of different shapes), and Color
* Voxel Operations: Add and Paint, Add (add voxels and don't set material/color), Subtract (remove voxels), and Paint Only (to only set Material / Color)
* Set the main <<glossary:Material Asset>>, and add additional materials to paint with.
[block:api-header]
{
  "title": "Smooth Mode or Cube Mode"
}
[/block]
Voxel volumes can either be in Smooth mode (using Marching Cubes algorithm to make a smooth mesh), or Cube mode for a Minecraft style voxels.
[block:image]
{
  "images": [
    {
      "image": [
        "https://files.readme.io/90aa03c-VoxelCube.PNG",
        "VoxelCube.PNG",
        3000,
        902,
        "#355863"
      ],
      "caption": "'Cube' mode on left, and 'Smooth' mode on right"
    }
  ]
}
[/block]

[block:api-header]
{
  "title": "Destruction"
}
[/block]
By default Voxels are destroyable by player damaging - including from Melee weapons / projectiles / explosions. This can be turned off in the Voxel settings.