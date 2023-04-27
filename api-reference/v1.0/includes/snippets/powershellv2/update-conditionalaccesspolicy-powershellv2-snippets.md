---
description: "Automatically generated file. DO NOT MODIFY"
---

```powershellv2

Import-Module Microsoft.Graph.Identity.SignIns

$params = @{
	conditions = @{
		signInRiskLevels = @(
			"high"
			"medium"
			"low"
		)
	}
}

Update-MgIdentityConditionalAccessPolicy -ConditionalAccessPolicyId $conditionalAccessPolicyId -BodyParameter $params

```