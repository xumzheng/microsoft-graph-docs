---
description: "Automatically generated file. DO NOT MODIFY"
---

```powershellv2

Import-Module Microsoft.Graph.Beta.Calendar

$params = @{
	Name = "Volunteer"
}

# A UPN can also be used as -UserId.
New-MgBetaUserCalendar -UserId $userId -BodyParameter $params

```