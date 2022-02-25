---
title: "Creating Components"
slug: "creating-components"
hidden: false
createdAt: "2021-06-17T22:58:40.665Z"
updatedAt: "2021-07-21T14:17:19.898Z"
---
* Add a new class that inherits from [ComponentEntity](doc:componententity) - and it will show as a add option ingame

* Entity Components are Unity MonoBehaviors, so Awake / Start / Update / FixedUpdate can all be used

* If using Awake, it needs to be overridden and and base.Awake() called- since the base component's Awake method needs to run

There are a few Modbox specific virtual methods that can be used:
* AfterAddedToWorld - Called after the Entity was added to World and Awake is called
* RefreshComponents - Called after added to world and whenever components are changed on the Entity. This is where any components should be set.
* SavedDataLoaded - Called after the Entity loads it's data, if it's saved in the world
* RefreshValuesBefore - If the component has values that can be changed by other components, it should 'refresh' them and clear them.
* RefreshValuesAfter - Where a component should change other components values (that got cleared in RefreshValuesBefore)
* OnPlaymodeStarted - Called on starting play mode but before Physics body created
* OnPlaymodeAfter - Called after physics body created and play mode started

Use 'GetComponentEntity' rather than 'GetComponent' - since components can also be added to the Entity by child gameobjects in some cases (like if  the entity has a [Humanoid Models](doc:humanoid-models) with Components)
[block:code]
{
  "codes": [
    {
      "code": "\n    [MBDescription(\"Draws a Line to show the Spring Joint.\")]\n    [MBTypeComponentEnabledInEditmode]\n    [MBTypeRequireComponents(typeof(EntSpringJoint))]\n    public class EntSpringJointLine : ComponentEntity\n    {\n        [MBValueOnChangedMethod(nameof(OnChange_Enabled))]\n        [MBValueDefaultValue(true)]\n        public BoolVariable Enabled { get; private set; }\n\n        [MBValueOnChangedMethod(nameof(OnChange_Color))]\n        public ColorVariable Color { get; private set; }",
      "language": "csharp"
    }
  ]
}
[/block]
* Use 'MBTypeRequireComponents' - not Unity's 'RequireComponent', to set what other components are required for the component type

* MBTypeComponentEnabledInEditmode is used so that the Update/Start methods are run in edit mode. By default Entity components are disabled in edit mode.