---
description: "Automatically generated file. DO NOT MODIFY"
---

```powershellv2

Import-Module Microsoft.Graph.Beta.Calendar

$params = @{
	Name = "name-value"
}

# A UPN can also be used as -UserId.
Update-MgBetaUserCalendarGroup -UserId $userId -CalendarGroupId $calendarGroupId -BodyParameter $params

```