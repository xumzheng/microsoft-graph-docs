---
description: "Automatically generated file. DO NOT MODIFY"
---

```powershellv1

Import-Module Microsoft.Graph.Identity.DirectoryManagement

$params = @{
	Id = "Engineering"
	Description = "Attributes for engineering team"
	MaxAttributesPerSet = 25
}

New-MgDirectoryAttributeSet -BodyParameter $params

```