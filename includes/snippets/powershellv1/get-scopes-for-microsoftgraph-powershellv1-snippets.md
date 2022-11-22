---
description: "Automatically generated file. DO NOT MODIFY"
---

```powershellv1

Import-Module Microsoft.Graph.Applications

Get-MgServicePrincipal -Filter "displayName eq 'Microsoft Graph'" -Property "id,displayName,appId,oauth2PermissionScopes" 

```