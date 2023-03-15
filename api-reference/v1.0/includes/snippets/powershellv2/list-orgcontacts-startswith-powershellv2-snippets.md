---
description: "Automatically generated file. DO NOT MODIFY"
---

```powershellv2

Import-Module Microsoft.Graph.Identity.DirectoryManagement

Get-MgContact -Filter "startswith(displayName,'A')" -CountVariable CountVar -Top 1 -Sort "displayName" -ConsistencyLevel eventual 


```