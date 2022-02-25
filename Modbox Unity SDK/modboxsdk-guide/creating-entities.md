---
title: "Creating Entities"
slug: "creating-entities"
hidden: false
createdAt: "2020-05-25T05:23:21.442Z"
updatedAt: "2020-11-04T21:58:48.788Z"
---
​To create a Entity prefabs from Unity prefabs in the Project view, select the prefab you want to create an entity from and right click it. Then select 'Modbox/Create Modbox Entity Prefab(s)'. You can also select multiple prefabs at once for quick creation. Along with the entity prefab a 'Entity Asset' will also be created that links to the prefab.

* 'Keep Prefab Connection' means the prefab is then kept as a nested prefab in the entity prefab.
* Entities should not have Rigidbodies - since Modbox will create Rigidbodies for it
* If it has Colliders - they need to be convex unless the entity is set to 'AlwaysKinematic'. This is because Unity does not allow non-convex colliders on dynamic rigidbodies. For complex static structures (like arches), where you want to not have a convex collider (where changing to convex would fill in holes in the collider), use 'AlwaysKinematic', which will set it to never be non Kinematic and always static.

For creating a Entity prefab from a gameobject added to the scene, right click on it in the hierarchy and select 'Modbox/Turn GameObject Into Entity Prefab'

Place your Entity prefab in your mod folder (usually in a 'Entities' folder, but not required). It should then show up as a option to build with.

## Entity Scale \ Position \ 'AutoScale'
Entities should be facing up (the Y direction). When placing in the Desktop Editor or with the 'Entity Brush' surface mode, it'll rotate based on the angle it's being placed on - so a 'rocket thruster' should have it's exhaust pointed up, a button/screen should have it's button/screen pointing up.
 
[block:image]
{
  "images": [
    {
      "image": [
        "https://files.readme.io/ae25407-Ramp_1.png",
        "Ramp (1).png",
        1489,
        951,
        "#74808c"
      ],
      "caption": "For best use of the grid/scaling system, the center / pivot point of the entity (at 0,0,0 position) for most entities should be the center of the Entity."
    }
  ]
}
[/block]

When a Entity prefab is selected the 1m bounds are shown with a cube wireframe. If the entity is a structure that is meant for the grid system - like any of the primitives - it should be centered in the 1 bounds and fit into it exactly. Then Autoscale in it's 'EntTransform' script can be set to 'By 1 Bounds', meaning it'll scale assuming the Entity is 1m size (so if the gridsize is set to 0.25, it'll just scale the Entity to 0.25).
[block:image]
{
  "images": [
    {
      "image": [
        "https://files.readme.io/075b738-Lever_1.png",
        "Lever (1).png",
        1151,
        946,
        "#2a4058"
      ],
      "caption": "For entities that are meant to always be placed on a surface / wall, the center should be the bottom center position."
    }
  ]
}
[/block]
By default when scaling the 'Max Render Bounds' will be used.  Most entities are 'Autoscaled' when creating ingame by a VR players to the VR players scale

## Icons
To generate Icons for the Entity, enter play mode in Modbox with the 'Enable Auto Icon Making' option in MBStartup on. It'll render the object and save as a sprite.

## Entity Components
Entities have a special Monobehavior type for components called 'ComponentEntity', and a inherited 'ComponentEntityWithVariables'. 

## Entity Group Asset
Entity prefabs can have more than one Entity in a single prefab. This is good if you want them to have different rigidbodies in play mode (such as a Spinner Hinge Joint object, which has a different body for the top and bottom, and connects them with a physics joint in play mode) - or have child components of the same type that should be editable (like multiple wheels on a car). See examples like HingeJoint / Spinner.

​