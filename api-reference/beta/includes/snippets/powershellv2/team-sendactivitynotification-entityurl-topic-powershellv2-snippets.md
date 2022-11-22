---
description: "Automatically generated file. DO NOT MODIFY"
---

```powershellv2

Import-Module Microsoft.Graph.Beta.Teams

$params = @{
	Topic = @{
		Source = "entityUrl"
		Value = "https://graph.microsoft.com/beta/teams/{teamId}/channels/{channelId}/tabs/{tabId}"
	}
	ActivityType = "reservationUpdated"
	PreviewText = @{
		Content = "You have moved up the queue"
	}
	Recipient = @{
		"@odata.type" = "microsoft.graph.aadUserNotificationRecipient"
		UserId = "569363e2-4e49-4661-87f2-16f245c5d66a"
	}
	TemplateParameters = @(
		@{
			Name = "reservationId"
			Value = "TREEE433"
		}
		@{
			Name = "currentSlot"
			Value = "23"
		}
	)
}

Send-MgBetaTeamActivityNotification -TeamId $teamId -BodyParameter $params

```