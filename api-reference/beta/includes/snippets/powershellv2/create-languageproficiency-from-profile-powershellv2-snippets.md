---
description: "Automatically generated file. DO NOT MODIFY"
---

```powershellv2

Import-Module Microsoft.Graph.Beta.People

$params = @{
	DisplayName = "Norwegian Bokmål"
	Tag = "nb-NO"
	Spoken = "nativeOrBilingual"
	Written = "nativeOrBilingual"
	Reading = "nativeOrBilingual"
}

# A UPN can also be used as -UserId.
New-MgBetaUserProfileLanguage -UserId $userId -BodyParameter $params

```