---
description: "Automatically generated file. DO NOT MODIFY"
---

```powershellv2

Import-Module Microsoft.Graph.Beta.Identity.DirectoryManagement

$params = @{
	Description = "Attributes for engineering team"
	MaxAttributesPerSet = 20
}

Update-MgBetaDirectoryAttributeSet -AttributeSetId $attributeSetId -BodyParameter $params

```