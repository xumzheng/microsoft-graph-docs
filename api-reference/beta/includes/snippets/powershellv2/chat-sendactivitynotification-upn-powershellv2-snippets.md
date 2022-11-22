---
description: "Automatically generated file. DO NOT MODIFY"
---

```powershellv2

Import-Module Microsoft.Graph.Beta.Teams

$params = @{
	Topic = @{
		Source = "entityUrl"
		Value = "https://graph.microsoft.com/beta/chats/{chatId}/messages/{messageId}"
	}
	ActivityType = "approvalRequired"
	PreviewText = @{
		Content = "Deployment requires your approval"
	}
	Recipient = @{
		"@odata.type" = "microsoft.graph.aadUserNotificationRecipient"
		UserId = "jacob@contoso.com"
	}
	TemplateParameters = @(
		@{
			Name = "approvalTaskId"
			Value = "2020AAGGTAPP"
		}
	)
}

Send-MgBetaChatActivityNotification -ChatId $chatId -BodyParameter $params

```