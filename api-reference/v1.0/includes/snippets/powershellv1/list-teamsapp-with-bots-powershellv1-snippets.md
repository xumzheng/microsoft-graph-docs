---
description: "Automatically generated file. DO NOT MODIFY"
---

```powershellv1

Import-Module Microsoft.Graph.Teams

Get-MgAppCatalogTeamApp -ExpandProperty "appDefinitions(`$expand=bot)" -Filter "appDefinitions/any(a:a/bot ne null)" 

```