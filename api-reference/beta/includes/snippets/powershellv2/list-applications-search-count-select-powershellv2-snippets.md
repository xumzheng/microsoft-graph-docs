---
description: "Automatically generated file. DO NOT MODIFY"
---

```powershellv2

Import-Module Microsoft.Graph.Beta.Applications

Get-MgBetaApplication -Search "displayName:Web" -CountVariable CountVar -Property "appId,identifierUris,displayName,publisherDomain,signInAudience" -ConsistencyLevel eventual 


```