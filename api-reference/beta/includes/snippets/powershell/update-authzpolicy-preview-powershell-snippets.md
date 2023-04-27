---
description: "Automatically generated file. DO NOT MODIFY"
---

```powershell

Import-Module Microsoft.Graph.Identity.SignIns

$params = @{
	enabledPreviewFeatures = @(
		"assignGroupsToRoles"
	)
}

Update-MgPolicyAuthorizationPolicy -AuthorizationPolicyId $authorizationPolicyId -BodyParameter $params

```