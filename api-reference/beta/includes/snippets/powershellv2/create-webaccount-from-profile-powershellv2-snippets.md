---
description: "Automatically generated file. DO NOT MODIFY"
---

```powershellv2

Import-Module Microsoft.Graph.Beta.People

$params = @{
	Description = "My Github contributions!"
	UserId = "innocenty.popov"
	Service = @{
		Name = "GitHub"
		WebUrl = "https://github.com"
	}
}

# A UPN can also be used as -UserId.
New-MgBetaUserProfileWebAccount -UserId $userId -BodyParameter $params

```