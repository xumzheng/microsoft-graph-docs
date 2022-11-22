---
description: "Automatically generated file. DO NOT MODIFY"
---

```powershellv1

Import-Module Microsoft.Graph.Identity.SignIns

$params = @{
	UserInputType = "textBox"
}

Update-MgIdentityB2CUserFlowUserAttributeAssignment -B2cIdentityUserFlowId $b2cIdentityUserFlowId -IdentityUserFlowAttributeAssignmentId $identityUserFlowAttributeAssignmentId -BodyParameter $params

```