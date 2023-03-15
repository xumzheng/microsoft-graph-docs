---
description: "Automatically generated file. DO NOT MODIFY"
---

```powershellv2

Import-Module Microsoft.Graph.Beta.DirectoryObjects

Get-MgBetaDirectoryObject -DirectoryObjectId $directoryObjectId -Filter "isof('microsoft.graph.user') or isof('microsoft.graph.group')" 

```