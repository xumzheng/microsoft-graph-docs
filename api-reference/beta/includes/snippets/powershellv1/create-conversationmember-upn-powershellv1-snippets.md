---
description: "Automatically generated file. DO NOT MODIFY"
---

```powershellv1

Import-Module Microsoft.Graph.Teams

$params = @{
	"@odata.type" = "#microsoft.graph.aadUserConversationMember"
	Roles = @(
		"owner"
	)
	"User@odata.bind" = "https://graph.microsoft.com/v1.0/users('jacob@contoso.com')"
}

New-MgTeamMember -TeamId $teamId -BodyParameter $params

```