---
description: "Automatically generated file. DO NOT MODIFY"
---

```powershellv2

Import-Module Microsoft.Graph.Identity.SignIns

$params = @{
	permissionType = "delegated"
	clientApplicationsFromVerifiedPublisherOnly = $true
}

New-MgPolicyPermissionGrantPolicyInclude -PermissionGrantPolicyId $permissionGrantPolicyId -BodyParameter $params

```