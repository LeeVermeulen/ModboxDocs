---
title: "Creating Asset Types"
slug: "creating-asset-types"
hidden: false
createdAt: "2020-10-31T14:38:52.243Z"
updatedAt: "2020-10-31T17:17:16.976Z"
---
New asset types can be created by inheriting from the 'ModAsset' class.

Here is a example of a 'Imported Audio' asset that inherited from the AssetAudioClip type - which just loads a imported .wav/.mp3 file.
[block:code]
{
  "codes": [
    {
      "code": "using System.Collections;\nusing System.Collections.Generic;\nusing UnityEngine;\nusing ModboxMain;\nusing ModboxMods.Core;\n\nnamespace ModboxMods.ImportAudio\n{\n    [MBTypeAssetImportFileOptionsAttribute(\"wav\", \"mp3\" )]\n    [MBSetDescription(\"Audio Clip from a wav/mp3 file\")]\n    public class AssetAudioclipFile : AssetAudioClip\n    {\n        protected override void OnLoadOrReloadAsCreationAsset()\n        {\n            if (!CreationAssetData.FilePathExists())\n            {\n                CreationAssetDataLoadingState = CreationAssetLocalState.MissingFiles;\n                return;\n            }\n\n            Clip = RuntimeAudioClipLoader.Manager.Load(CreationAssetData.FileNamePath, false, false);\n        }\n    }\n}",
      "language": "csharp"
    }
  ]
}
[/block]