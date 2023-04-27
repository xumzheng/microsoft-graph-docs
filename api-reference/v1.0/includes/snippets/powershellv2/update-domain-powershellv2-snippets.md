---
description: "Automatically generated file. DO NOT MODIFY"
---

```powershellv2

Import-Module Microsoft.Graph.Identity.DirectoryManagement

$params = @{
	isDefault = $true
	supportedServices = @(
		"Email"
		"OfficeCommunicationsOnline"
	)
}

Update-MgDomain -DomainId $domainId -BodyParameter $params

```