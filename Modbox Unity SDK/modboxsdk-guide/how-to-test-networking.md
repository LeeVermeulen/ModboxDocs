---
title: "How To Test Networking"
slug: "how-to-test-networking"
hidden: false
createdAt: "2020-05-25T16:43:41.335Z"
updatedAt: "2021-06-17T23:42:52.860Z"
---
Easiest way to test Modbox C# networking is to open the same Modbox Unity project in another Unity Editor. This way any changes you make to the project will update both editors. Unity doesn't allow you to open the same project folder - but you can get around this by creating symbolic links of the Assets / ProjectSettings in another folder, and opening that (so assets / project settings are shared, but the generated library/temp stuff is not)

To create a new Project Folder with Symbolic links - use 'Create Symlink Project Clone' option in the Modbox menu