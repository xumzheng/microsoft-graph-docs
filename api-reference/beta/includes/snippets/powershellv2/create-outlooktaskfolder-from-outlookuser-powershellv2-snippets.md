---
description: "Automatically generated file. DO NOT MODIFY"
---

```powershellv2

Import-Module Microsoft.Graph.Beta.Users

$params = @{
	Name = "Volunteer"
}

# A UPN can also be used as -UserId.
New-MgBetaUserOutlookTaskFolder -UserId $userId -BodyParameter $params

```