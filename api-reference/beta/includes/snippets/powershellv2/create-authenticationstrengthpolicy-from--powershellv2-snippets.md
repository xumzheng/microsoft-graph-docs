---
description: "Automatically generated file. DO NOT MODIFY"
---

```powershellv2

Import-Module Microsoft.Graph.Beta.Identity.SignIns

$params = @{
	"@odata.type" = "#microsoft.graph.authenticationStrengthPolicy"
	DisplayName = "Contoso authentication level"
	Description = "The only authentication level allowed to access our secret apps"
	AllowedCombinations = @(
		"password, hardwareOath"
		"password, sms"
	)
}

New-MgBetaPolicyAuthenticationStrengthPolicy -BodyParameter $params

```