---
description: "Automatically generated file. DO NOT MODIFY"
---

```powershellv2

Import-Module Microsoft.Graph.Beta.Identity.SignIns

$params = @{
	Definition = @(
		"{"TokenLifetimePolicy":{"Version":1,"AccessTokenLifetime":"8:00:00"}}"
	)
	DisplayName = "Contoso token lifetime policy"
	IsOrganizationDefault = $true
}

New-MgBetaPolicyTokenLifetimePolicy -BodyParameter $params

```