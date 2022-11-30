---
description: "Automatically generated file. DO NOT MODIFY"
---

```powershellv2

Import-Module Microsoft.Graph.Beta.Applications

$params = @{
	PermissionId = "e1fe6dd8-ba31-4d61-89e7-88639da4683d"
	PermissionName = "User.Read"
	Classification = "low"
}

New-MgBetaServicePrincipalDelegatedPermissionClassification -ServicePrincipalId $servicePrincipalId -BodyParameter $params

```