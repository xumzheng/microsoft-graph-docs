---
description: "Automatically generated file. DO NOT MODIFY"
---

```powershellv1

Import-Module Microsoft.Graph.Calendar

$params = @{
	OriginalStartTimeZone = "originalStartTimeZone-value"
	OriginalEndTimeZone = "originalEndTimeZone-value"
	ResponseStatus = @{
		Response = ""
		Time = [System.DateTime]::Parse("datetime-value")
	}
	Uid = "iCalUId-value"
	ReminderMinutesBeforeStart = 99
	IsReminderOn = $true
}

Update-MgGroupEvent -GroupId $groupId -EventId $eventId -BodyParameter $params

```