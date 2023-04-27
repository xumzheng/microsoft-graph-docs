---
description: "Automatically generated file. DO NOT MODIFY"
---

```powershell

Import-Module Microsoft.Graph.Identity.SignIns

$params = @{
	id = "Customer"
	userFlowType = "signUpOrSignIn"
	userFlowTypeVersion = 3
	identityProviders = @(
		@{
			id = "Facebook-OAuth"
		}
	)
}

New-MgIdentityB2CUserFlow -BodyParameter $params

```