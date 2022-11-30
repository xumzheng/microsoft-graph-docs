---
description: "Automatically generated file. DO NOT MODIFY"
---

```powershellv2

Import-Module Microsoft.Graph.Beta.Identity.SignIns

$params = @{
	IsOptional = $false
	RequiresVerification = $false
	UserInputType = "TextBox"
	DisplayName = "Shoe size"
	UserAttributeValues = @(
	)
	UserAttribute = @{
		Id = "extension_guid_shoeSize"
	}
}

New-MgBetaIdentityB2CUserFlowUserAttributeAssignment -B2cIdentityUserFlowId $b2cIdentityUserFlowId -BodyParameter $params

```