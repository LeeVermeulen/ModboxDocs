---
title: "Code Access"
slug: "whitelist"
hidden: false
createdAt: "2021-07-03T15:06:28.645Z"
updatedAt: "2021-07-03T21:02:43.590Z"
---
For security in loading mods / creations with C# code, only some namespaces are allowed to be accessed. Along with this there are a few Unity methods that are restricted (Application.Quit, PlayerPrefs.DeleteAll)

For any security issues or exploits found - email: [contact@alientrap.org](mailto:contact@alientrap.org) 
[block:api-header]
{
  "title": "NameSpace Whitelist"
}
[/block]
            "ModboxMain",
            "ModboxMain.MBScript",
            "ModboxMods.*",
            "UnityEngine",
            "UnityEngine.UI",
            "UnityEngine.EventSystems",
            "UnityEngine.Collections",
            "Pathfinding",
            "System",
            "System.Collections",
            "System.Collections.Generic",
            "System.Collections.ObjectModel",
            "System.Linq",
            "System.Convert",
            "Billboards"