---
description: "Automatically generated file. DO NOT MODIFY"
---

```powershellv2

Import-Module Microsoft.Graph.Beta.People

$params = @{
	Categories = @(
		"Sports"
	)
	Description = "World's greatest football club"
	DisplayName = "Chelsea FC"
	WebUrl = "https://www.chelseafc.com"
}

# A UPN can also be used as -UserId.
New-MgBetaUserProfileInterest -UserId $userId -BodyParameter $params

```