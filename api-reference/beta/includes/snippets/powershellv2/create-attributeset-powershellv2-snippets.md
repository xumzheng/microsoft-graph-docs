---
description: "Automatically generated file. DO NOT MODIFY"
---

```powershellv2

Import-Module Microsoft.Graph.Beta.Identity.DirectoryManagement

$params = @{
	Id = "Engineering"
	Description = "Attributes for engineering team"
	MaxAttributesPerSet = 25
}

New-MgBetaDirectoryAttributeSet -BodyParameter $params

```