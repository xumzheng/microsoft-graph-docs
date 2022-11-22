---
description: "Automatically generated file. DO NOT MODIFY"
---

```powershellv2

Import-Module Microsoft.Graph.Beta.People

$params = @{
	AllowedAudiences = "contacts"
}

# A UPN can also be used as -UserId.
Update-MgBetaUserProfileAnniversary -UserId $userId -PersonAnnualEventId $personAnnualEventId -BodyParameter $params

```