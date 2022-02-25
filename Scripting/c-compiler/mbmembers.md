---
title: "Functions\\Extensions"
slug: "mbmembers"
hidden: false
createdAt: "2020-05-26T05:57:27.287Z"
updatedAt: "2021-07-21T14:21:52.568Z"
---
* [MBFunction] attribute can be used on static methods to have them as Function options in MBScript
* 'MBFunctionForType' attribute can be used to set it to show under another type

* Static C# methods can be exposed as Extensions for <<glossary:MBScript>> / <<glossary:Wiring>>, where the first Parameter type is then what it's a extension for (like C# extension methods)

[block:code]
{
  "codes": [
    {
      "code": "\n[MBExtension]\nstatic int Length(string Text)\n{\n    if (Text == null)\n        return 0;\n    return Text.Length;\n}\n\n[MBFunctionQuickOption]\n[MBFunctionForType(typeof(string))]\nstatic string NewLine()\n{\n    return System.Environment.NewLine;\n}",
      "language": "text"
    }
  ]
}
[/block]
* The 'NewLine' can then be used in MBScript like: Func.String.NewLine

* The 'Length' extension can be used on any value returning a string. Like 'Name.Length'