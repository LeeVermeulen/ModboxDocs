---
title: "EntHingeJointMotor"
slug: "enthingejointmotor"
hidden: false
createdAt: "2020-11-10T21:59:50.143Z"
updatedAt: "2021-06-18T01:37:49.695Z"
---
**Hinge Joint Motor**
Causes a Hinge Joint to rotate.

ID: EntHingeJointMotor
Requires Components: [Hinge Joint](doc:enthingejoint)
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
    "0-0": "Motor",
    "0-1": "Bool Variable",
    "0-2": "",
    "1-0": "Motor Speed",
    "1-1": "Number Variable",
    "1-2": "The motor's target speed.The speed of the motor is influenced by the mass of the connected entity, so if the Motor Force is too low it may be unable to reach the set speed. - degrees/s",
    "2-0": "Set Target Angle",
    "2-1": "Bool Variable",
    "2-2": "",
    "3-0": "Spring Force",
    "3-1": "Number Variable",
    "3-2": "The force of the spring used to reach the target angle.This force is influenced by the mass of the connected entity, so if the Spring Force is too low it may be unable to reach the target angle. - kn",
    "4-0": "Spring Damper",
    "4-1": "Number Variable",
    "4-2": "The spring's damper. This effects the speed that the spring moves at.Higher values will make the spring move more slowly, but help prevent it from overshooting it's target. - kn",
    "5-0": "Target Angle",
    "5-1": "Number Variable",
    "5-2": "The target angle. Note that this is effected by the joint limit on the Hinge Joint component. - degrees",
    "6-0": "Motor Force",
    "6-1": "Number Variable",
    "6-2": "How fast the motor is able to spin the joint. This influences how quickly the motor will reach it's set speed. - kn",
    "7-0": "Reverse",
    "7-1": "Bool Variable",
    "7-2": "",
    "8-0": "Pendulum",
    "8-1": "Bool Variable",
    "8-2": "Swings like a pendulum between min/max angles",
    "9-0": "Pendulum Reversed",
    "9-1": "Bool Variable",
    "9-2": " - ReadOnly"
  },
  "cols": 3,
  "rows": 10
}
[/block]