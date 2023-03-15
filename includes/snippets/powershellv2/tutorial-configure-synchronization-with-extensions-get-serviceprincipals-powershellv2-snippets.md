---
description: "Automatically generated file. DO NOT MODIFY"
---

```powershellv2

Import-Module Microsoft.Graph.Beta.Applications

Get-MgBetaServicePrincipal -Property "id,appId,displayName" -Filter "startswith(displayName, 'salesforce')" 

```