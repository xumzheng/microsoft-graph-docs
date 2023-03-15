---
description: "Automatically generated file. DO NOT MODIFY"
---

```powershellv2

Import-Module Microsoft.Graph.Beta.Users.Actions

$params = @{
	NewReminderTime = @{
		DateTime = "2016-10-19T10:37:00Z"
		TimeZone = "timeZone-value"
	}
}

# A UPN can also be used as -UserId.
Invoke-MgBetaSnoozeUserEventReminder -UserId $userId -EventId $eventId -BodyParameter $params

```