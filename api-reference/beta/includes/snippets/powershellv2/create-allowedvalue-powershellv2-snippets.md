---
description: "Automatically generated file. DO NOT MODIFY"
---

```powershellv2

Import-Module Microsoft.Graph.Beta.Identity.DirectoryManagement

$params = @{
	id = "Alpine"
	isActive = "true"
}

New-MgBetaDirectoryCustomSecurityAttributeDefinitionAllowedValue -CustomSecurityAttributeDefinitionId $customSecurityAttributeDefinitionId -BodyParameter $params

```