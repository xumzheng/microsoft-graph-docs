---
description: "Automatically generated file. DO NOT MODIFY"
---

```powershellv2

Import-Module Microsoft.Graph.Groups

Get-MgGroupMember -GroupId $groupId -CountVariable CountVar -Filter "startswith(displayName, 'a')" -ConsistencyLevel eventual 


```