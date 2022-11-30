---
description: "Automatically generated file. DO NOT MODIFY"
---

```powershellv1

Import-Module Microsoft.Graph.Identity.SignIns

$params = @{
	LocalizedStrings = @(
	)
}

Set-MgIdentityB2CUserFlowLanguageOverridePageContent -B2cIdentityUserFlowId $b2cIdentityUserFlowId -UserFlowLanguageConfigurationId $userFlowLanguageConfigurationId -UserFlowLanguagePageId $userFlowLanguagePageId -BodyParameter $params

```