---
description: "Automatically generated file. DO NOT MODIFY"
---

```powershellv2

Import-Module Microsoft.Graph.Beta.Calendar

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

Update-MgBetaGroupEvent -GroupId $groupId -EventId $eventId -BodyParameter $params

```