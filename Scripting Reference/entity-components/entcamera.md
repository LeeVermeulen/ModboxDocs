---
title: "EntCamera"
slug: "entcamera"
hidden: false
createdAt: "2020-11-10T22:11:20.111Z"
updatedAt: "2021-06-18T01:37:38.146Z"
---
**Camera**
Renders a camera view, which can then be hooked up to a screen

ID: EntCamera
Required By: [Camera Post FX](doc:entcamerapostfx)
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
    "0-0": "Camera On",
    "0-1": "Bool Variable",
    "0-2": "Defaults to True",
    "1-0": "Draw To Screen",
    "1-1": "Bool Variable",
    "1-2": "If true the camera will display on the screen, displaying on top of the user's camera.",
    "2-0": "Viewport Position",
    "2-1": "Vector2 Variable",
    "2-2": "The origin position of the camera display on screen. These values represent a percentage of the screen where(0, 0) is the bottom left, and(1, 1) is the top right. Note that the camera's origin will always be in the bottom left of the viewport, so setting the viewport's x or y value to 1 will cause it to display offscreen.",
    "3-0": "Viewport Size",
    "3-1": "Vector2 Variable",
    "3-2": "The size of the camera display on the screen. These values represent the percentage of the screen that is covered, so for example a value of (0.3, 0.5) would cover 30% of the screen's width and 50% of the screen's height.",
    "4-0": "FPS",
    "4-1": "Enum Variable<Cam FPS Type>",
    "4-2": "The camera's Frames Per-Second. - Defaults to _30",
    "5-0": "FOV",
    "5-1": "Number Variable",
    "5-2": "The camera's Field of View. - Defaults to 60 - degrees",
    "6-0": "Resolution",
    "6-1": "Vector2 Variable",
    "6-2": "",
    "7-0": "Hide Side Screen",
    "7-1": "Bool Variable",
    "7-2": "Hides the 'SideScreen' part of the model if this was on a Entity with a camera model"
  },
  "cols": 3,
  "rows": 8
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
    "0-0": "Preview UI",
    "0-1": "",
    "0-2": ""
  },
  "cols": 2,
  "rows": 1
}
[/block]