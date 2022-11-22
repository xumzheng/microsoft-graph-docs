---
description: "Automatically generated file. DO NOT MODIFY"
---

```powershellv1

Import-Module Microsoft.Graph.Users

Get-MgUser -Search "displayName:wa" OR "displayName:ad" -Sort "displayName" -CountVariable CountVar -ConsistencyLevel eventual 


```