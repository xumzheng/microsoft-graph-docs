---
description: "Automatically generated file. DO NOT MODIFY"
---

```powershellv2

Import-Module Microsoft.Graph.Calendar

$params = @{
	Role = "write"
}

Update-MgUserCalendarPermission -UserId $userId -CalendarPermissionId $calendarPermissionId -BodyParameter $params

```