---
description: "Automatically generated file. DO NOT MODIFY"
---

```powershellv2

Import-Module Microsoft.Graph.Identity.SignIns

$params = @{
	defaultUserRolePermissions = @{
		permissionGrantPoliciesAssigned = @(
			"managePermissionGrantsForSelf.microsoft-user-default-low"
		)
	}
}

Update-MgPolicyAuthorizationPolicy -BodyParameter $params

```