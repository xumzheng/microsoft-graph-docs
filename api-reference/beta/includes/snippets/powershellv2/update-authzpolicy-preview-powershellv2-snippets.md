---
description: "Automatically generated file. DO NOT MODIFY"
---

```powershellv2

Import-Module Microsoft.Graph.Beta.Identity.SignIns

$params = @{
	enabledPreviewFeatures = @(
		"assignGroupsToRoles"
	)
}

Update-MgBetaPolicyAuthorizationPolicy -AuthorizationPolicyId $authorizationPolicyId -BodyParameter $params

```