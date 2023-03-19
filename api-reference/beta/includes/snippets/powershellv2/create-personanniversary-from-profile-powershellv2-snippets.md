---
description: "Automatically generated file. DO NOT MODIFY"
---

```powershellv2

Import-Module Microsoft.Graph.Beta.People

$params = @{
	Type = "birthday"
	Date = "1980-01-08"
}

# A UPN can also be used as -UserId.
New-MgBetaUserProfileAnniversary -UserId $userId -BodyParameter $params

```