---
description: "Automatically generated file. DO NOT MODIFY"
---

```powershellv1

Import-Module Microsoft.Graph.People

$params = @{
	Description = "Lyn Damer play in the Women's 1st Division (Toppserien) in Norway"
}

# A UPN can also be used as -UserId.
Update-MgUserProfileWebsite -UserId $userId -PersonWebsiteId $personWebsiteId -BodyParameter $params

```