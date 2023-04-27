---
description: "Automatically generated file. DO NOT MODIFY"
---

```powershellv2

Import-Module Microsoft.Graph.Beta.People

$params = @{
	allowedAudiences = "organization"
	countryCode = "NO"
}

# A UPN can also be used as -UserId.
New-MgBetaUserProfileAccount -UserId $userId -BodyParameter $params

```