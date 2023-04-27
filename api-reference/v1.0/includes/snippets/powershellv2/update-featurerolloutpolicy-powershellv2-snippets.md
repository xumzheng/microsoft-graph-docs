---
description: "Automatically generated file. DO NOT MODIFY"
---

```powershellv2

Import-Module Microsoft.Graph.Identity.SignIns

$params = @{
	displayName = "PasswordHashSync Rollout Policy"
	description = "PasswordHashSync Rollout Policy"
	isEnabled = $true
	isAppliedToOrganization = $false
}

Update-MgPolicyFeatureRolloutPolicy -FeatureRolloutPolicyId $featureRolloutPolicyId -BodyParameter $params

```