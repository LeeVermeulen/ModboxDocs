---
title: "C# Compiler Mod"
slug: "c-compiler-mod"
hidden: false
createdAt: "2020-10-31T00:20:25.273Z"
updatedAt: "2021-07-21T14:15:21.829Z"
---
[block:callout]
{
  "type": "info",
  "body": "C# Compiler mod currently not public - still in testing"
}
[/block]
* The C# Compiler mod allows for creating C# components at Runtime. Which can include new Entity Components, world settings, editor tools, new asset types and import options - or any functionality that a mod can include.
* VisualStudio or any C# editor can be used. Compiling is done while playing, and any changes / types are reloaded.
* Some Namespaces (such as System.IO) are restricted from use for Creation C# code.
* C# Projects are included in creations as <<glossary:Asset>>s, and can be included in Prefabs to share online

* The Project 'Mod_Core' is included in the VisualStudio project (the source for the Core Modbox mod, with all the editor tools / main components).