---
title: "Adding to UI"
slug: "adding-to-ui"
hidden: false
createdAt: "2020-05-26T05:54:42.526Z"
updatedAt: "2021-06-17T22:57:35.752Z"
---
* For Variables on [MBSingleton](doc:mbsingleton) - use MBUICategory and MBUIGroup to set what category the variable should show in in the UI.

Attributes can be used to set how the widget should show
[block:code]
{
  "codes": [
    {
      "code": "[MBValueMinFloatAttribute(0)]\n[MBValueMaxFloatAttribute(5)]\n[MBValueSlider(WholeNumbers: true, HideEditNumpad: true)]\npublic FloatVariable QualityLevel { get; private set; }",
      "language": "text"
    }
  ]
}
[/block]
## Register UI Buttons
Separate from the MBVariable system is a way to register UI buttons with the settings systems. This is a way to include buttons in the various Settings windows. A icon can be set, SetVisible can be used to set when it should be shown, and 'OnClick' for when it is clicked.
[block:code]
{
  "codes": [
    {
      "code": "RegisteredUIButton BuildNewButton = new RegisteredUIButton(\"Build New\", this, ButtonIcons.Instance.BuildNew);\nSettingsVars.RegisterUIButton(BuildNewButton, \"MainMenu\");\nBuildNewButton.SetVisible = () =>\n{\n     return !Engine.Instance.InOnlineRoom;\n};\nBuildNewButton.OnClicked = () =>\n{\n      BuildNewButton.BigUI.ShowScreen(\"BuildNewScreen\");\n};",
      "language": "csharp"
    }
  ]
}
[/block]