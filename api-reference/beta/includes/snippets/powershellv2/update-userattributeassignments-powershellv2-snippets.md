---
description: "Automatically generated file. DO NOT MODIFY"
---

```powershellv2

Import-Module Microsoft.Graph.Beta.Identity.SignIns

$params = @{
	UserInputType = "textBox"
}

Update-MgBetaIdentityB2CUserFlowUserAttributeAssignment -B2cIdentityUserFlowId $b2cIdentityUserFlowId -IdentityUserFlowAttributeAssignmentId $identityUserFlowAttributeAssignmentId -BodyParameter $params

```