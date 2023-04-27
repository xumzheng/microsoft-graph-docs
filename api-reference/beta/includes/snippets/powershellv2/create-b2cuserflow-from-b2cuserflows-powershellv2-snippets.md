---
description: "Automatically generated file. DO NOT MODIFY"
---

```powershellv2

Import-Module Microsoft.Graph.Beta.Identity.SignIns

$params = @{
	id = "Customer"
	userFlowType = "signUpOrSignIn"
	userFlowTypeVersion = 3
}

New-MgBetaIdentityB2CUserFlow -BodyParameter $params

```