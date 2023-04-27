---
description: "Automatically generated file. DO NOT MODIFY"
---

```powershellv2

Import-Module Microsoft.Graph.Identity.SignIns

$params = @{
	displayName = "Hobby"
	description = "Your hobby"
	dataType = "string"
}

New-MgIdentityUserFlowAttribute -BodyParameter $params

```