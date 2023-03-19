---
description: "Automatically generated file. DO NOT MODIFY"
---

```powershellv2

Import-Module Microsoft.Graph.Beta.Identity.SignIns

$params = @{
	NewAssignmentOrder = @{
		Order = @(
			"City"
			"extension_GUID_ShoeSize"
		)
	}
}

Set-MgBetaIdentityB2CUserFlowUserAttributeAssignmentOrder -B2cIdentityUserFlowId $b2cIdentityUserFlowId -BodyParameter $params

```