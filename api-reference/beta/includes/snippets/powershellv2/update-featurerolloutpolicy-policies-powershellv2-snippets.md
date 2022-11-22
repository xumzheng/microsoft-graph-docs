---
description: "Automatically generated file. DO NOT MODIFY"
---

```powershellv2

Import-Module Microsoft.Graph.Beta.Identity.SignIns

$params = @{
	DisplayName = "PasswordHashSync Rollout Policy"
	Description = "PasswordHashSync Rollout Policy"
	IsEnabled = $true
	IsAppliedToOrganization = $false
}

Update-MgBetaPolicyFeatureRolloutPolicy -FeatureRolloutPolicyId $featureRolloutPolicyId -BodyParameter $params

```