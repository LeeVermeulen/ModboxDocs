---
title: "MBSingleton"
slug: "mbsingleton"
hidden: false
createdAt: "2020-10-31T14:39:08.017Z"
updatedAt: "2021-07-21T14:22:24.721Z"
---
MBSingleton can be used to create a C# singleton to access through other scripts.

Use the 'MBSingletonCreateOnLoad' attribute to have the Singleton instance created on the code/mod loaded.

MBSingleton's with [MBVariables](doc:mbvariables) need a 'MBMemberLocation' attribute. This will set where the values will be saved (with the World, or Creation, Or Server, or as a Preference)
[block:code]
{
  "codes": [
    {
      "code": "[MBUICategory(\"Game\")]\n[MBUIGroup(\"AI\")]\n[MBMemberLocation(MBMemberLocation.World)]\t// save values with each world\npublic class AStarPathfindingSystem : MBSingleton<AStarPathfindingSystem>\n{\n    public BoolVariable UsePathfinding { get; private set; }\n}",
      "language": "text"
    }
  ]
}
[/block]
Unlike some Unity singleton patterns they are not auto created on use. They are set when added to the world - then set to null on Destroyed


[block:code]
{
  "codes": [
    {
      "code": "using ModboxMain;\n\nnamespace ModboxMods.Core\n{\n    public class CorePlayersSystem : MBSingleton<CorePlayersSystem>\n    {\n      \t// MBVariable events\n        [MBParameterNames(\"player\")]\n        public EventVariable<EntMBPlayer> MBPlayerJoined { get; private set; }\n\n        [MBParameterNames(\"player\")]\n        public EventVariable<EntMBPlayer> MBPlayerLeft { get; private set; }\n\n      \t// MBVariable Value that will show in the world settings under 'Game'\n        [MBShowInSettingWindow( SettingsWindow.World, \"Game\", \"Rules\")]\n        [MBDefaultValueAttribute(true)]\n        public BoolVariable AddPlayerNameTags { get; private set; }\n      \n        protected override void Awake()\n        {\n          \t// always use base.Awake with MBSingleton\n            base.Awake();\n          \n          \t// add a UI button on how to play\n            RegisteredUIButton helpButton = new RegisteredUIButton(\"How To Play\", this, IconFiles.Instance.Help);\n            SettingsVars.ShowButtonInWindow(helpButton, SettingsWindow.MainMenu);\n            helpButton.SetButtonVisible = () =>\n            {\n                return MBGameState.InLobby;\n            };\n            helpButton.OnClicked = () =>\n            {\n                UIScreenTutorials tutorials = helpButton.LastUIScreenCanvas.ShowScreenByType<UIScreenTutorials>();\n                tutorials.HideEditTutorials();\n                tutorials.Intro.isOn = true;\n            };\n          \n            EntMBPlayer.Event_MBPlayerJoined.AddListener(OnEvent_MBPlayerJoined);\n            EntMBPlayer.Event_MBPlayerLeft.AddListener(OnEvent_MBPlayerLeft);\n        }\n      \n        void OnEvent_MBPlayerLeft(EntMBPlayerBase player)\n        {\n            MBPlayerLeft.RunEventLocal(player as EntMBPlayer);\n        }\n\n        void OnEvent_MBPlayerJoined(EntMBPlayerBase player)\n        {\n            MBPlayerJoined.RunEventLocal(player as EntMBPlayer);\n        }\n    }\n}",
      "language": "csharp"
    }
  ]
}
[/block]