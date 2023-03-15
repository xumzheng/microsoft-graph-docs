---
description: "Automatically generated file. DO NOT MODIFY"
---

```powershellv2

Import-Module Microsoft.Graph.Beta.Users

Get-MgBetaUser -CountVariable CountVar -Property "id,displayName,customSecurityAttributes" -Filter "startsWith(customSecurityAttributes/Marketing/EmployeeId,'GS')" -ConsistencyLevel eventual 


```