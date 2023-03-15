---
description: "Automatically generated file. DO NOT MODIFY"
---

```powershellv2

Import-Module Microsoft.Graph.Beta.Teams

$params = @{
	"@odata.type" = "#microsoft.graph.aadUserConversationMember"
	"User@odata.bind" = "https://graph.microsoft.com/beta/users/jacob@contoso.com"
	VisibleHistoryStartDateTime = [System.DateTime]::Parse("2019-04-18T23:51:43.255Z")
	Roles = @(
		"owner"
	)
}

New-MgBetaChatMember -ChatId $chatId -BodyParameter $params

```