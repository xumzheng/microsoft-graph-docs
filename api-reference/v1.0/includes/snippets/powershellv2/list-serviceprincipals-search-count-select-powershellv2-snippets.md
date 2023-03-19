---
description: "Automatically generated file. DO NOT MODIFY"
---

```powershellv2

Import-Module Microsoft.Graph.Applications

Get-MgServicePrincipal -Search "displayName:Team" -CountVariable CountVar -Property "accountEnabled,displayName,publisherName,servicePrincipalType,signInAudience" -ConsistencyLevel eventual 


```