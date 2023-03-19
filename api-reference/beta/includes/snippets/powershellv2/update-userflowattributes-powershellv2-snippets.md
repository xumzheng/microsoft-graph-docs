---
description: "Automatically generated file. DO NOT MODIFY"
---

```powershellv2

Import-Module Microsoft.Graph.Beta.Identity.SignIns

$params = @{
	Description = "Your new hobby"
}

Update-MgBetaIdentityUserFlowAttribute -IdentityUserFlowAttributeId $identityUserFlowAttributeId -BodyParameter $params

```