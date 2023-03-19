---
description: "Automatically generated file. DO NOT MODIFY"
---

```powershellv2

Import-Module Microsoft.Graph.DirectoryObjects

Get-MgDirectoryObject -DirectoryObjectId $directoryObjectId -Filter "isof('microsoft.graph.user') or isof('microsoft.graph.group')" 

```