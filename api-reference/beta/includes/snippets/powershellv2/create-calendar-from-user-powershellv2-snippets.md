---
description: "Automatically generated file. DO NOT MODIFY"
---

```powershellv2

Import-Module Microsoft.Graph.Beta.Calendar

$params = @{
	name = "Volunteer"
}

# A UPN can also be used as -UserId.
New-MgBetaUserCalendar -UserId $userId -BodyParameter $params

```