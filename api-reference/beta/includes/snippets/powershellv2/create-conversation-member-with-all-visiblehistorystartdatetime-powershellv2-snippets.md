---
description: "Automatically generated file. DO NOT MODIFY"
---

```powershellv2

Import-Module Microsoft.Graph.Beta.Teams

$params = @{
	"@odata.type" = "#microsoft.graph.aadUserConversationMember"
	"User@odata.bind" = "https://graph.microsoft.com/beta/users/8b081ef6-4792-4def-b2c9-c363a1bf41d5"
	VisibleHistoryStartDateTime = [System.DateTime]::Parse("0001-01-01T00:00:00Z")
	Roles = @(
		"owner"
	)
}

New-MgBetaChatMember -ChatId $chatId -BodyParameter $params

```