---
description: "Automatically generated file. DO NOT MODIFY"
---

```powershellv2

Import-Module Microsoft.Graph.Beta.Identity.DirectoryManagement

$params = @{
	isDefault = $true
	supportedServices = @(
		"Email"
		"OfficeCommunicationsOnline"
	)
}

Update-MgBetaDomain -DomainId $domainId -BodyParameter $params

```