---
description: "Automatically generated file. DO NOT MODIFY"
---

```powershell

Import-Module Microsoft.Graph.Identity.SignIns

$params = @{
	id = "UserFlowWithAPIConnector"
	userFlowType = "signUpOrSignIn"
	userFlowTypeVersion = 1
	apiConnectorConfiguration = @{
		postFederationSignup = @{
			"@odata.id" = "{apiConnectorId}"
		}
		postAttributeCollection = @{
			"@odata.id" = "{apiConnectorId}"
		}
	}
}

New-MgIdentityB2XUserFlow -BodyParameter $params

```