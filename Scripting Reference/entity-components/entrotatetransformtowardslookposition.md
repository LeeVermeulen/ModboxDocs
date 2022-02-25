---
title: "EntRotateTransformTowardsLookPosition"
slug: "entrotatetransformtowardslookposition"
hidden: false
createdAt: "2020-11-10T21:51:06.800Z"
updatedAt: "2021-06-18T01:38:02.092Z"
---
**Rotate Transform Towards Look Position**
Rotates a transform on the entity towards the Movement component's look position.

ID: EntRotateTransformTowardsLookPosition
Requires Components: [Movement](doc:entmovement)
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
    "0-0": "Rotate Speed",
    "0-1": "Number Variable",
    "0-2": "x",
    "1-0": "Rotate Part",
    "1-1": "Transform Part Variable",
    "1-2": "The transform that will be rotated.",
    "2-0": "Aim With Part",
    "2-1": "Transform Part Variable",
    "2-2": "If set the RotatePart will be rotated so this part is aimed. This should be a child of RotatePart"
  },
  "cols": 3,
  "rows": 3
}
[/block]