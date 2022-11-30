---
description: "Automatically generated file. DO NOT MODIFY"
---

```powershellv1

Import-Module Microsoft.Graph.People

$params = @{
	Description = "My Github contributions!"
	UserId = "innocenty.popov"
	Service = @{
		Name = "GitHub"
		WebUrl = "https://github.com"
	}
}

# A UPN can also be used as -UserId.
New-MgUserProfileWebAccount -UserId $userId -BodyParameter $params

```