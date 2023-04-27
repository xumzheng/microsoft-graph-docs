---
description: "Automatically generated file. DO NOT MODIFY"
---

```powershellv2

Import-Module Microsoft.Graph.Identity.SignIns

$params = @{
	userInputType = "textBox"
}

Update-MgIdentityB2XUserFlowUserAttributeAssignment -B2xIdentityUserFlowId $b2xIdentityUserFlowId -IdentityUserFlowAttributeAssignmentId $identityUserFlowAttributeAssignmentId -BodyParameter $params

```