---
description: "Automatically generated file. DO NOT MODIFY"
---

```powershell

Import-Module Microsoft.Graph.Identity.SignIns

$params = @{
	permissionGrantPolicyIdsAssignedToDefaultUserRole = @(
		"managePermissionGrantsForSelf.microsoft-user-default-low"
	)
}

Update-MgPolicyAuthorizationPolicy -AuthorizationPolicyId $authorizationPolicyId -BodyParameter $params

```