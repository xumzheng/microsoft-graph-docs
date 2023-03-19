---
description: "Automatically generated file. DO NOT MODIFY"
---

```powershellv2

Import-Module Microsoft.Graph.Beta.Applications

Get-MgBetaApplication -Filter "owners/`$count eq 0 or owners/`$count eq 1" -CountVariable CountVar -Property "id,displayName" -ConsistencyLevel eventual 


```