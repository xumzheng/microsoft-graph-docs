---
description: "Automatically generated file. DO NOT MODIFY"
---

```powershellv2

Import-Module Microsoft.Graph.Beta.Users

Get-MgBetaUser -Search "displayName:wa" OR "displayName:ad" -Sort "displayName" -CountVariable CountVar -ConsistencyLevel eventual 


```