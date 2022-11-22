---
description: "Automatically generated file. DO NOT MODIFY"
---

```powershellv2

Import-Module Microsoft.Graph.Beta.Identity.SignIns

$params = @{
	DisplayName = "New Test API"
	TargetUrl = "https://otherapi.com/api/endpoint"
	AuthenticationConfiguration = @{
		"@odata.type" = "microsoft.graph.basicAuthentication"
		Username = "<NEW_USERNAME>"
		Password = "<NEW_PASSWORD>"
	}
}

Update-MgBetaIdentityApiConnector -IdentityApiConnectorId $identityApiConnectorId -BodyParameter $params

```