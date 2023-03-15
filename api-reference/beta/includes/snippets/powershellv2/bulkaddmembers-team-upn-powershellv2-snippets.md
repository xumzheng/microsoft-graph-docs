---
description: "Automatically generated file. DO NOT MODIFY"
---

```powershellv2

Import-Module Microsoft.Graph.Beta.Teams

$params = @{
	Values = @(
		@{
			"@odata.type" = "microsoft.graph.aadUserConversationMember"
			Roles = @(
			)
			"User@odata.bind" = "https://graph.microsoft.com/beta/users('jacob@contoso.com')"
		}
		@{
			"@odata.type" = "microsoft.graph.aadUserConversationMember"
			Roles = @(
				"owner"
			)
			"User@odata.bind" = "https://graph.microsoft.com/beta/users('alex@contoso.com')"
		}
	)
}

Add-MgBetaTeamsMember -TeamId $teamId -BodyParameter $params

```