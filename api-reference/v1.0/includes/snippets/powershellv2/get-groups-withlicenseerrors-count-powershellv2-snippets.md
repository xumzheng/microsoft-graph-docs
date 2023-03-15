---
description: "Automatically generated file. DO NOT MODIFY"
---

```powershellv2

Import-Module Microsoft.Graph.Groups

Get-MgGroup -CountVariable CountVar -Filter "hasMembersWithLicenseErrors eq true" -Property "id,displayName" -ConsistencyLevel eventual 


```