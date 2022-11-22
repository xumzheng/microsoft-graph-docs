---
description: "Automatically generated file. DO NOT MODIFY"
---

```powershellv1

Import-Module Microsoft.Graph.Identity.SignIns

$params = @{
	Description = "Your new hobby"
}

Update-MgIdentityUserFlowAttribute -IdentityUserFlowAttributeId $identityUserFlowAttributeId -BodyParameter $params

```