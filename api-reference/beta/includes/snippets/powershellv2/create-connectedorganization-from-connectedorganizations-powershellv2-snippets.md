---
description: "Automatically generated file. DO NOT MODIFY"
---

```powershellv2

Import-Module Microsoft.Graph.Beta.Identity.Governance

$params = @{
	DisplayName = "Connected organization name"
	Description = "Connected organization description"
	IdentitySources = @(
		@{
			"@odata.type" = "#microsoft.graph.domainIdentitySource"
			DomainName = "example.com"
			DisplayName = "example.com"
		}
	)
	State = "proposed"
}

New-MgBetaEntitlementManagementConnectedOrganization -BodyParameter $params

```