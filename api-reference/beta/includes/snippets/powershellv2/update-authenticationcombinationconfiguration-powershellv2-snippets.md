---
description: "Automatically generated file. DO NOT MODIFY"
---

```powershellv2

Import-Module Microsoft.Graph.Beta.Identity.SignIns

$params = @{
	AppliesToCombinations = @(
		"fido2"
	)
}

Update-MgBetaIdentityConditionalAccessAuthenticationStrengthPolicyCombinationConfiguration -AuthenticationStrengthPolicyId $authenticationStrengthPolicyId -AuthenticationCombinationConfigurationId $authenticationCombinationConfigurationId -BodyParameter $params

```