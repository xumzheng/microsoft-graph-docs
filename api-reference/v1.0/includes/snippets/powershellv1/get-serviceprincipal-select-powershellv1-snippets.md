---
description: "Automatically generated file. DO NOT MODIFY"
---

```powershellv1

Import-Module Microsoft.Graph.Applications

Get-MgServicePrincipal -ServicePrincipalId $servicePrincipalId -Property "id,appId,displayName,appRoles,oauth2PermissionScopes" 

```