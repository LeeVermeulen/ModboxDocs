---
title: "Properties"
slug: "properties"
hidden: false
createdAt: "2021-06-17T21:47:51.888Z"
updatedAt: "2021-07-03T17:34:42.189Z"
---
* To expose C# Properties ingame add a [MBMember] or [MBReadOnly] attribute
[block:code]
{
  "codes": [
    {
      "code": "[MBReadOnly]\n[MBSuffix(\"x\")]\n[MBDescription(\"Percentage of health to Start health\")]\n[MBHideWidgetIfDefault]\npublic float HealthPercentage => Health.Value / StartHealth.Value;",
      "language": "csharp"
    }
  ]
}
[/block]
'HideWidgetIfDefault' can be used to not show the value if it's default (0 for numbers, empty/null for strings)

Can also use [MBMember] on Methods:
[block:code]
{
  "codes": [
    {
      "code": "\n[MBMember]\npublic void ClearTargetAndMoveGoal()\n{\n    MoveGoalWorldPosition.SetValueOnline(Vector3.zero);\n    MoveGoalEntity.SetValueOnline(null);\n    MoveGoalRange.SetValueOnline(Range.Zero);\n    Target.SetValueOnline(null);\n}",
      "language": "csharp"
    }
  ]
}
[/block]
Should only use this on Methods that don't need to be called on all clients (in this example the value variables are synced). Otherwise should use a 'OnlineVoidMethod' [MBVariables](doc:mbvariables)