---
description: "Automatically generated file. DO NOT MODIFY"
---

```powershellv2

Import-Module Microsoft.Graph.Applications

$params = @{
	appRoleAssignmentRequired = $true
}

Update-MgServicePrincipal -ServicePrincipalId $servicePrincipalId -BodyParameter $params

```