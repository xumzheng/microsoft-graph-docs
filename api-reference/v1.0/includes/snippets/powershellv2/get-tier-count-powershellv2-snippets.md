---
description: "Automatically generated file. DO NOT MODIFY"
---

```powershellv2

Import-Module Microsoft.Graph.Groups

Get-MgGroupTransitiveMember -GroupId $groupId -DirectoryObjectId $directoryObjectId -CountVariable CountVar -Sort "displayName" -Search "displayName:tier" -Property "displayName,id" -ConsistencyLevel eventual 


```