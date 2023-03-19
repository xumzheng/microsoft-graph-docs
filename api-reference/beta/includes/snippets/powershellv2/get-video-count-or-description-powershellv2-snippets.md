---
description: "Automatically generated file. DO NOT MODIFY"
---

```powershellv2

Import-Module Microsoft.Graph.Beta.Groups

Get-MgBetaGroup -Search "displayName:Video" OR "description:prod" -Sort "displayName" -CountVariable CountVar -ConsistencyLevel eventual 


```