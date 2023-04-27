---
description: "Automatically generated file. DO NOT MODIFY"
---

```powershellv2

Import-Module Microsoft.Graph.Beta.Applications

$params = @{
	appRoleAssignmentRequired = $true
}

Update-MgBetaServicePrincipal -ServicePrincipalId $servicePrincipalId -BodyParameter $params

```