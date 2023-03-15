---
description: "Automatically generated file. DO NOT MODIFY"
---

```powershellv2

Import-Module Microsoft.Graph.Identity.SignIns

$params = @{
	Definition = @(
		"definition-value"
	)
	DisplayName = "displayName-value"
	IsOrganizationDefault = $true
}

Update-MgPolicyTokenIssuancePolicy -TokenIssuancePolicyId $tokenIssuancePolicyId -BodyParameter $params

```