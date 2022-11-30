---
description: "Automatically generated file. DO NOT MODIFY"
---

```powershellv2

Import-Module Microsoft.Graph.Groups

Get-MgGroup -Property "id,assignedLicenses" -Filter "assignedLicenses/any()" 

```