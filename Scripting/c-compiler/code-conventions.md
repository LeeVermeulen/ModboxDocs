---
title: "Code Conventions"
slug: "code-conventions"
hidden: false
createdAt: "2020-05-25T06:09:56.047Z"
updatedAt: "2020-11-15T22:12:42.513Z"
---
## Script Naming:

* New Entity components should be 'Ent[NAME].cs', Tool scripts should be 'Tool[NAME].cs'. Asset types should start with 'Asset'

## Entity Components

* Variables for the Unity inspector should be at the top - and should generally be private with a '[SerializeField]' if not needing to be public.
* When Lerping or changing a position over time, need to use Time.fixedDeltaTime if in FixedUpdate, and Time.DeltaTime if in Coroutine/Update. Like Mathf.Lerp(OldValue, NewValue, 10 * Time.fixedDeltaTime). This is because FixedDeltaTime will change (depending on Platform / Viewmode, in VR the FixedDeltaTime is usually higher)

## Unity C#

* Functionality should be split into as many Components as possible, with little dependency between them. Communication can be done with the Events / MBVariables
* Avoid all allocation in Update/FixedUpdate/LateUpdate/Coroutines (anything that runs each frame). Allocations include 'GetComponents' calls
* Avoid use of Update / LateUpdate / FixedUpdate when possible, for any script there could be a lot of active instances of. Usually using events + coroutines can replace needing to constantly run Update to check/respond to things

## C#

Generally follow these C# Guidelines: http://wiki.unity3d.com/index.php/Csharp_Coding_Guidelines  --

* New line for braces

* Use camelCasing for private member variables, parameters, and local variables. 
* Use PascalCasing for public fields/methods/enums/property/event/class names

* Generally comments are only needed to describe something where code isn't enough (a hacky approach, a workaround, explaining a complex algorithm)

* Properties should not include a lot of hidden processing. In general, a property { get; set;} method should not then call a Method, like a hidden GetComponent / AddComponent

* Always prefer to check against null and use a '==' operator. So if checking for null, do not just use 'if (obj) ', which is unclear, use 'if (obj != null)'