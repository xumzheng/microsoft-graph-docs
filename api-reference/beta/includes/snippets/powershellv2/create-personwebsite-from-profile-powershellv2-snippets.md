---
description: "Automatically generated file. DO NOT MODIFY"
---

```powershellv2

Import-Module Microsoft.Graph.Beta.People

$params = @{
	Categories = @(
		"football"
	)
	DisplayName = "Lyn Damer"
	WebUrl = "www.lyndamer.no"
}

# A UPN can also be used as -UserId.
New-MgBetaUserProfileWebsite -UserId $userId -BodyParameter $params

```