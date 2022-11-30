---
description: "Automatically generated file. DO NOT MODIFY"
---

```powershellv2

Import-Module Microsoft.Graph.Beta.Applications

$params = @{
	AppRoleAssignmentRequired = $true
}

Update-MgBetaServicePrincipal -ServicePrincipalId $servicePrincipalId -BodyParameter $params

```