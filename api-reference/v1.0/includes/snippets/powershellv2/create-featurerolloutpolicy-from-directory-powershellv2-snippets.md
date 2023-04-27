---
description: "Automatically generated file. DO NOT MODIFY"
---

```powershellv2

Import-Module Microsoft.Graph.Identity.SignIns

$params = @{
	displayName = "PassthroughAuthentication rollout policy"
	description = "PassthroughAuthentication rollout policy"
	feature = "passthroughAuthentication"
	isEnabled = $true
	isAppliedToOrganization = $false
}

New-MgPolicyFeatureRolloutPolicy -BodyParameter $params

```