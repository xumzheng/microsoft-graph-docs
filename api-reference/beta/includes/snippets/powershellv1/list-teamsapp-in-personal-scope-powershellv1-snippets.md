---
description: "Automatically generated file. DO NOT MODIFY"
---

```powershellv1

Import-Module Microsoft.Graph.Teams

Get-MgAppCatalogTeamApp -ExpandProperty "appDefinitions(`$select=id,displayName,allowedInstallationScopes)" -Filter "appDefinitions/any(a:a/allowedInstallationScopes has 'personal')" 

```