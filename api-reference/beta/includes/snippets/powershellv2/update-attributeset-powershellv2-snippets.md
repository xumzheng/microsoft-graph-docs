---
description: "Automatically generated file. DO NOT MODIFY"
---

```powershellv2

Import-Module Microsoft.Graph.Beta.Identity.DirectoryManagement

$params = @{
	description = "Attributes for engineering team"
	maxAttributesPerSet = 20
}

Update-MgBetaDirectoryAttributeSet -AttributeSetId $attributeSetId -BodyParameter $params

```