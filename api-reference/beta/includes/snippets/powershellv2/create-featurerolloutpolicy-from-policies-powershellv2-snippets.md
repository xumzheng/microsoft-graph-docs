---
description: "Automatically generated file. DO NOT MODIFY"
---

```powershellv2

Import-Module Microsoft.Graph.Beta.Identity.SignIns

$params = @{
	DisplayName = "PassthroughAuthentication rollout policy"
	Description = "PassthroughAuthentication rollout policy"
	Feature = "passthroughAuthentication"
	IsEnabled = $true
	IsAppliedToOrganization = $false
}

New-MgBetaPolicyFeatureRolloutPolicy -BodyParameter $params

```