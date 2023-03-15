---
description: "Automatically generated file. DO NOT MODIFY"
---

```powershellv2

Import-Module Microsoft.Graph.Beta.Groups

Get-MgBetaGroupTransitiveMember -GroupId $groupId -DirectoryObjectId $directoryObjectId -CountVariable CountVar -Sort "displayName" -Filter "startswith(displayName, 'a')" -ConsistencyLevel eventual 


```