---
description: "Automatically generated file. DO NOT MODIFY"
---

```powershellv2

Import-Module Microsoft.Graph.Beta.People

$params = @{
	Nickname = "Kesha"
}

# A UPN can also be used as -UserId.
Update-MgBetaUserProfileName -UserId $userId -PersonNameId $personNameId -BodyParameter $params

```