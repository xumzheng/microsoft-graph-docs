---
description: "Automatically generated file. DO NOT MODIFY"
---

```powershellv2

Import-Module Microsoft.Graph.Beta.Teams

$params = @{
	DisplayName = "My First Shared Channel"
	Description = "This is my first shared channel"
	MembershipType = "shared"
	Members = @(
		@{
			"@odata.type" = "#microsoft.graph.aadUserConversationMember"
			"User@odata.bind" = "https://graph.microsoft.com/beta/users('7640023f-fe43-gv3f-9gg4-84a9efe4acd6')"
			Roles = @(
				"owner"
			)
		}
	)
}

New-MgBetaTeamChannel -TeamId $teamId -BodyParameter $params

```