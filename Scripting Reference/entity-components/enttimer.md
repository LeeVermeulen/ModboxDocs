---
title: "EntTimer"
slug: "enttimer"
hidden: false
createdAt: "2020-11-10T21:51:06.575Z"
updatedAt: "2021-06-18T01:38:02.335Z"
---
**Timer**
Countdown / Timelimit timer

ID: EntTimer
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
    "0-0": "Enabled",
    "0-1": "Bool Variable",
    "0-2": "Defaults to True",
    "1-0": "Mode",
    "1-1": "Enum Variable<Timer Mode>",
    "1-2": "",
    "2-0": "Time",
    "2-1": "Number Variable",
    "2-2": "Defaults to 30 - s",
    "3-0": "Stop At Time",
    "3-1": "Number Variable",
    "3-2": "Enabled will be set to False on time hit - s"
  },
  "cols": 3,
  "rows": 4
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
    "0-0": "Reset Time()",
    "0-1": "Resets Time to what it was at start of Play mode, and sets Enabled to True"
  },
  "cols": 2,
  "rows": 1
}
[/block]

[block:api-header]
{
  "title": "Events"
}
[/block]

[block:parameters]
{
  "data": {
    "h-0": "Name",
    "h-1": "Description",
    "0-0": "Time Stopped()",
    "0-1": ""
  },
  "cols": 2,
  "rows": 1
}
[/block]