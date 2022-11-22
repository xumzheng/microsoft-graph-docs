---
description: "Automatically generated file. DO NOT MODIFY"
---

```powershellv1

Import-Module Microsoft.Graph.Identity.SignIns

$params = @{
	PermissionType = "delegated"
	CertifiedClientApplicationsOnly = $true
}

New-MgPolicyPermissionGrantPolicyInclude -PermissionGrantPolicyId $permissionGrantPolicyId -BodyParameter $params

```