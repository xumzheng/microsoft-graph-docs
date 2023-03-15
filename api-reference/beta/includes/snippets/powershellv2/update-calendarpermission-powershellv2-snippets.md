---
description: "Automatically generated file. DO NOT MODIFY"
---

```powershellv2

Import-Module Microsoft.Graph.Beta.Calendar

$params = @{
	Role = "write"
}

Update-MgBetaUserCalendarPermission -UserId $userId -CalendarPermissionId $calendarPermissionId -BodyParameter $params

```