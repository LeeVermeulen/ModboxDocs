---
title: "MBVariables"
slug: "mbvariables"
hidden: false
createdAt: "2020-05-25T05:28:27.941Z"
updatedAt: "2021-07-21T14:21:16.454Z"
---
MBVariables are how all entity/assets/world values and methods are saved in the creation, synced online, edited, animated, and connected together with visual scripting.

They are created automatically for [ComponentEntity](doc:componententity) / [MBSingleton](doc:mbsingleton) on Awake, and on load for [Asset Types](doc:creating-asset-types)

They should be added as Properties with a { get; private set }
[block:code]
{
  "codes": [
    {
      "code": "using ModboxMain;\nusing UnityEngine;\n\nnamespace ModboxMods.Core\n{\n    [MBSetDescriptionAttribute(\"Will die on impact above a min velocity\")]\n    public class EntDieOnImpact : ComponentEntityWithVariables\n    {\n        [MBSetSuffix(\"m/s\")]\n        [MBSetDescription(\"Minimum speed the entity should die on collision\")]\n        [MBValueOnChangedMethod(nameof(OnChange_TooltipScale))]\n        public FloatVariable MinVelocity { get; private set; }\n\n        protected override void Awake()\n        {\n            base.Awake();\n            WorldEnt.Event_OnCollisionEnter.AddListener(EntEvent_OnCollisionEnter);\n        }\n\n        void OnChange_MinVelocity()\n        {\n            // The velocity changed! Add code here to run on value changed\n        }\n\n        void EntEvent_OnCollisionEnter(Collision Coll, ContactPoint Contact)\n        {\n            if (Coll.relativeVelocity.magnitude > MinVelocity.Value)\n            {\n                EntMain.Die.RunOnline();\n            }\n        }\n    }\n}\n",
      "language": "csharp"
    }
  ]
}
[/block]
For variables to hold/sync data there is a MBVariableValue type for that data type. For saving a number FloatVariable is used, StringVariable for text, and ColorVariable for color. There is also MBVariableValue types for all the different kind of assets that can be included in mods - such as EntityAssetVariable and MaterialVariable. There are also types that store references to world entities and components, such as EntityVariable.

Some MBVariable types that store values have a 'Real Type' (for the EntityAssetVariable this would be a Entity asset), and a 'Saved Type' (for EntityAssetVariable this would be a string, 'Cube|main', saying the asset name and the mod it's from). The 'Saved Type' is what is synced online and serialized.

MBVariables have different 'Locations'. They can be on Entities (their value is saved with the entity), or in the World, or on a asset (saved as changes to that asset in the creation), or as a player preference (saved with the player's preferences).

**Setting/Getting values**: The 'Value' gives the value. Use 'SetValueOnline' to set the value and send that value online for other clients to also set. Use 'SetValueLocal' when just setting the value only on the local machine.

* **MBValueOnChangedMethod** attribute can be used to have a method run when the value is changed.
**OnValueChanged Event:** Can use 'Event_OnValueChanged.AddListener ' to have methods run when variables from other components change there value. There is no need to remove a listener, since it'll be removed when the script is destroyed (there is also a 'RemoveListener' function to remove it before that).

[block:code]
{
  "codes": [
    {
      "code": "IsOn.Event_OnValueChanged.AddListener(IsOnChanged); // IsOnChanged is a method to run when the value changes",
      "language": "csharp"
    }
  ]
}
[/block]
**UI Editing:** How MBVariables show in the UI to edit depends on their type (floats can show as sliders, enums as dropdowns, strings as text fields, prefabs with a button to open a prefab browser). There are some Attributes that can be set on the variable to set how it's shown (for a float, min/max slider values).


## OnlineVoidMethod
To add a Method that should run online - add a 'OnlineVoidMethod' variable - and set the method it should call in it's attribute.
Changes to MBVariables should then use 'SetValueLocal' (since the method is already running on all clients, changes dont need to be synced)
[block:code]
{
  "codes": [
    {
      "code": "[OnlineMethod(nameof(HealHealth_Called))]\npublic OnlineVoidMethod<float> HealHealth { get; private set; }\n\nvoid HealHealth_Called(float Amount)\n{\n        Health.SetValueLocal(Health.Value + Amount);\n}",
      "language": "csharp"
    }
  ]
}
[/block]


## Event Variables
EventVariables can be used to expose a event to scripting (so scripting can be added when that event happens). Such as in the event of a physics collision, 'EventVariable<WorldEntity> OnCollision', that is run with 'OnCollision.RunActionLocal(OtherWorldEnt)'. 'OnCollision' will then be a event option with visual scripting (with WorldEntity as a given parameter).

'RunEventOnline' should be used when a event happens on a client that might not be the master client (and that action wouldn't happen on the MasterClient) - it will then send the action to the MasterClient (if it isn't the MasterClient) to run the visual scripting event. This shouldn't be used for something like physics collisions - since that should be checked on the MasterClient.

[Return Value Events](doc:return-value-events)  variables can be used to get a value from MBScript, and can run on all clients (so the result of the 'ReturnValueVariable' set by MBScript is immediate and doesn't need to wait for a response from the MasterClient)

## Lists
MBVariable values can also be stored as lists of values, rather than just a single value. Use the '[MBValueList]' attributeto have the MBVariable be a list.

[block:code]
{
  "codes": [
    {
      "code": "\n[MBValueList]\npublic StringVariable Tags { get; private set; }\n\nvoid Start()\n{\n\tTags.List.ListAddElement(\"NewTag\", true);\n}",
      "language": "text"
    }
  ]
}
[/block]
'.List.ValueList' can then be used to get a read only collection of the values.

Other
Missing Values: A MBVariable has a 'Saved Value' but can't find it's 'Real Value'. This could mean it's saved value is 'Rifle' (a string saying its the rifle entity prefab), but since it can't find that value the real value is missing. Another example would be the 'EntityVariable', which could have a saved value of a entity id number (like '37335'), but since that entity doesn't exist in the world it would be missing. 'IsRealValueMissing' bool can check for this.