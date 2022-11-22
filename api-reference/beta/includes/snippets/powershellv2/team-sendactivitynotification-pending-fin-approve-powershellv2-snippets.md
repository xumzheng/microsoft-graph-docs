---
description: "Automatically generated file. DO NOT MODIFY"
---

```powershellv2

Import-Module Microsoft.Graph.Beta.Teams

$params = @{
	Topic = @{
		Source = "entityUrl"
		Value = "https://graph.microsoft.com/beta/teams/e8bece96-d393-4b9b-b8da-69cedef1a7e7"
	}
	ActivityType = "pendingFinanceApprovalRequests"
	PreviewText = @{
		Content = "Internal spending team has a pending finance approval requests"
	}
	Recipient = @{
		"@odata.type" = "microsoft.graph.teamMembersNotificationRecipient"
		TeamId = "e8bece96-d393-4b9b-b8da-69cedef1a7e7"
	}
	TemplateParameters = @(
		@{
			Name = "pendingRequestCount"
			Value = "5"
		}
	)
}

Send-MgBetaTeamActivityNotification -TeamId $teamId -BodyParameter $params

```