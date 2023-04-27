---
description: "Automatically generated file. DO NOT MODIFY"
---

```powershellv2

Import-Module Microsoft.Graph.Beta.Identity.SignIns

$params = @{
	id = "Partner"
	userFlowType = "signUpOrSignIn"
	userFlowTypeVersion = 1
	identityProviders = @(
		@{
			id = "Facebook-OAuth"
			type = "Facebook"
			name = "Facebook"
		}
	)
}

New-MgBetaIdentityB2XUserFlow -BodyParameter $params

```