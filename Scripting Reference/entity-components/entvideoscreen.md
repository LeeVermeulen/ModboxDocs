---
title: "EntVideoScreen"
slug: "entvideoscreen"
hidden: false
createdAt: "2020-11-10T21:51:06.922Z"
updatedAt: "2021-06-18T01:38:07.720Z"
---
**Video Screen**
Can play VideoFiles, CameraFeed, or a URL

ID: EntVideoScreen
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
    "0-0": "Source",
    "0-1": "Enum Variable<Video Screen Source>",
    "0-2": "",
    "1-0": "Camera Feed",
    "1-1": "Entity Component Variable<Camera>",
    "1-2": "",
    "2-0": "Mirror",
    "2-1": "Bool Variable",
    "2-2": "",
    "3-0": "Video Asset",
    "3-1": "Video File Variable",
    "3-2": "",
    "4-0": "Video URL",
    "4-1": "Text Variable",
    "4-2": "Note that this requires a direct URL to the video. URLs to video player sites such as Youtube won't work.",
    "5-0": "Loop",
    "5-1": "Bool Variable",
    "5-2": "",
    "6-0": "Paused",
    "6-1": "Bool Variable",
    "6-2": "",
    "7-0": "Volume",
    "7-1": "Number Variable",
    "7-2": "Defaults to 1 - x"
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
    "0-0": "Restart Video()",
    "0-1": ""
  },
  "cols": 2,
  "rows": 1
}
[/block]

[block:api-header]
{
  "title": "Properties"
}
[/block]

[block:parameters]
{
  "data": {
    "h-0": "Name",
    "h-1": "Type",
    "h-2": "Description",
    "0-0": "Play Time",
    "0-1": "Number",
    "0-2": "",
    "1-0": "Is Playing",
    "1-1": "Bool",
    "1-2": ""
  },
  "cols": 3,
  "rows": 2
}
[/block]


Attributes:
ModboxMain.MBTypeComponentNoIngameAddingAttribute