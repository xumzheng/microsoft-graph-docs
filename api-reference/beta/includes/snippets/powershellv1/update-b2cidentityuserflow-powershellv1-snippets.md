---
description: "Automatically generated file. DO NOT MODIFY"
---

```powershellv1

Import-Module Microsoft.Graph.Identity.SignIns

$params = @{
	IsLanguageCustomizationEnabled = $true
	DefaultLanguageTag = "en"
}

Update-MgIdentityB2CUserFlow -B2cIdentityUserFlowId $b2cIdentityUserFlowId -BodyParameter $params

```