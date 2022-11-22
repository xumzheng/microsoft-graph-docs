---
description: "Automatically generated file. DO NOT MODIFY"
---

```powershellv1

Import-Module Microsoft.Graph.Identity.DirectoryManagement

$params = @{
	Description = "Attributes for engineering team"
	MaxAttributesPerSet = 20
}

Update-MgDirectoryAttributeSet -AttributeSetId $attributeSetId -BodyParameter $params

```