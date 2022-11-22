---
description: "Automatically generated file. DO NOT MODIFY"
---

```powershellv2

Import-Module Microsoft.Graph.Beta.Users

$params = @{
	BusinessPhones = @(
		"+1 425 555 0109"
	)
	OfficeLocation = "18/2111"
}

# A UPN can also be used as -UserId.
Update-MgBetaUser -UserId $userId -BodyParameter $params

```