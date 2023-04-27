---
description: "Automatically generated file. DO NOT MODIFY"
---

```powershellv2

Import-Module Microsoft.Graph.Calendar

$params = @{
	role = "write"
}

Update-MgUserCalendarPermission -UserId $userId -CalendarPermissionId $calendarPermissionId -BodyParameter $params

```