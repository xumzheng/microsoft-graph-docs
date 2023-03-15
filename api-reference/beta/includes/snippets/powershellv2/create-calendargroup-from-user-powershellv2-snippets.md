---
description: "Automatically generated file. DO NOT MODIFY"
---

```powershellv2

Import-Module Microsoft.Graph.Beta.Calendar

$params = @{
	Name = "Personal events"
}

# A UPN can also be used as -UserId.
New-MgBetaUserCalendarGroup -UserId $userId -BodyParameter $params

```