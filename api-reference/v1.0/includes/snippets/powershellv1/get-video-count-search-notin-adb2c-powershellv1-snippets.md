---
description: "Automatically generated file. DO NOT MODIFY"
---

```powershellv1

Import-Module Microsoft.Graph.Groups

Get-MgGroup -Search "displayName:Video" OR "description:prod" -Sort "displayName" -CountVariable CountVar -ConsistencyLevel eventual 


```