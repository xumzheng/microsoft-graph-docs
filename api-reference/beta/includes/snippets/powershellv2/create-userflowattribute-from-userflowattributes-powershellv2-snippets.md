---
description: "Automatically generated file. DO NOT MODIFY"
---

```powershellv2

Import-Module Microsoft.Graph.Beta.Identity.SignIns

$params = @{
	DisplayName = "Hobby"
	Description = "Your hobby"
	DataType = "string"
}

New-MgBetaIdentityUserFlowAttribute -BodyParameter $params

```