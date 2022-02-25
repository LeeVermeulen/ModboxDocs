---
title: "EntAnimatedHumanoid"
slug: "entanimatedhumanoid"
hidden: false
createdAt: "2020-11-10T22:11:20.127Z"
updatedAt: "2021-06-18T01:35:57.423Z"
---
**Animated Humanoid**
On any non-VR Humanoid NPCs/Players

ID: EntAnimatedHumanoid
Requires Components: [Walking Movement](doc:entwalkingmovement), [Movement](doc:entmovement), [Humanoid](doc:enthumanoid)
Required By: [Holder Hand Animated](doc:entholderhandanimated), [Holder Hand Animated Left](doc:entholderhandanimatedleft), [Holder Hand Animated Right](doc:entholderhandanimatedright), [Animated Humanoid Bone Physics](doc:entanimatedhumanoidbonephysics), [Animated Humanoid Loop](doc:entanimatedhumanoidloop)
Base Type: [Entity Component](doc:componententity)

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
    "0-0": "Crouching",
    "0-1": "Bool Variable",
    "0-2": "",
    "1-0": "Melee Strafing",
    "1-1": "Bool Variable",
    "1-2": ""
  },
  "cols": 3,
  "rows": 2
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
    "0-0": "Do Anim Trigger(Humanoid Animation Trigger anim, Bool leftSide)",
    "0-1": "",
    "1-0": "Play Animation(Animation Clip Humanoid clip, Bool torsoOnly, Number speed)",
    "1-1": "",
    "2-0": "Stop Animation()",
    "2-1": ""
  },
  "cols": 2,
  "rows": 3
}
[/block]


Attributes:
ModboxMain.MBTypeComponentNoIngameAddingAttribute