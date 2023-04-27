---
description: "Automatically generated file. DO NOT MODIFY"
---

```powershellv2

Import-Module Microsoft.Graph.Groups

$params = @{
	originalStartTimeZone = "originalStartTimeZone-value"
	originalEndTimeZone = "originalEndTimeZone-value"
	iCalUId = "iCalUId-value"
	reminderMinutesBeforeStart = 99
	isReminderOn = $true
}

Update-MgGroupThread -GroupId $groupId -ConversationThreadId $conversationThreadId -BodyParameter $params

```