---
description: "Automatically generated file. DO NOT MODIFY"
---

```powershell

Import-Module Microsoft.Graph.Identity.SignIns

$params = @{
	permissionGrantPolicyIdsAssignedToDefaultUserRole = @(
	)
}

Update-MgPolicyAuthorizationPolicy -AuthorizationPolicyId $authorizationPolicyId -BodyParameter $params

```