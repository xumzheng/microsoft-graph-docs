---
description: "Automatically generated file. DO NOT MODIFY"
---

```powershellv2

Import-Module Microsoft.Graph.Users.Actions

$params = @{
	Id = "id-value"
	GroupId = "groupId-value"
	RenameAs = "renameAs-value"
}

# A UPN can also be used as -UserId.
Copy-MgUserOnenoteSectionToNotebook -UserId $userId -OnenoteSectionId $onenoteSectionId -BodyParameter $params

```