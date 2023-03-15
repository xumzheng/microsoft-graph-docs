---
description: "Automatically generated file. DO NOT MODIFY"
---

```powershellv2

Import-Module Microsoft.Graph.Beta.Teams

$params = @{
	"@odata.type" = "#Microsoft.Graph.channel"
	MembershipType = "private"
	DisplayName = "My First Private Channel"
	Description = "This is my first private channels"
	Members = @(
		@{
			"@odata.type" = "#microsoft.graph.aadUserConversationMember"
			"User@odata.bind" = "https://graph.microsoft.com/beta/users('62855810-484b-4823-9e01-60667f8b12ae')"
			Roles = @(
				"owner"
			)
		}
	)
}

New-MgBetaTeamChannel -TeamId $teamId -BodyParameter $params

```