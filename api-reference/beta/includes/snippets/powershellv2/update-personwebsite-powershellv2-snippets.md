---
description: "Automatically generated file. DO NOT MODIFY"
---

```powershellv2

Import-Module Microsoft.Graph.Beta.People

$params = @{
	Description = "Lyn Damer play in the Women's 1st Division (Toppserien) in Norway"
}

# A UPN can also be used as -UserId.
Update-MgBetaUserProfileWebsite -UserId $userId -PersonWebsiteId $personWebsiteId -BodyParameter $params

```