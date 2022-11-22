---
description: "Automatically generated file. DO NOT MODIFY"
---

```powershellv1

Import-Module Microsoft.Graph.Identity.SignIns

$params = @{
	AppliesToCombinations = @(
		"fido2"
	)
}

Update-MgIdentityConditionalAccessAuthenticationStrengthPolicyCombinationConfiguration -AuthenticationStrengthPolicyId $authenticationStrengthPolicyId -AuthenticationCombinationConfigurationId $authenticationCombinationConfigurationId -BodyParameter $params

```