---
description: "Automatically generated file. DO NOT MODIFY"
---

```powershellv2

Import-Module Microsoft.Graph.Beta.People

$params = @{
	DisplayName = "Innocenty Popov"
	First = "Innocenty"
	Initials = "IP"
	Last = "Popov"
	LanguageTag = "en-US"
	Maiden = $null
}

# A UPN can also be used as -UserId.
New-MgBetaUserProfileName -UserId $userId -BodyParameter $params

```