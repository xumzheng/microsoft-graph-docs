---
description: "Automatically generated file. DO NOT MODIFY"
---

```powershellv2

Import-Module Microsoft.Graph.Beta.Groups

$params = @{
	originalStartTimeZone = "originalStartTimeZone-value"
	originalEndTimeZone = "originalEndTimeZone-value"
	uid = "iCalUId-value"
	reminderMinutesBeforeStart = 99
	isReminderOn = $true
}

Update-MgBetaGroupThread -GroupId $groupId -ConversationThreadId $conversationThreadId -BodyParameter $params

```