---
description: "Automatically generated file. DO NOT MODIFY"
---

```powershell

Import-Module Microsoft.Graph.Teams

$params = @{
	"TeamsApp@odata.bind" = "https://graph.microsoft.com/beta/appCatalogs/teamsApps/7023576d-9e40-47ca-9cf2-daae6838e785"
	ConsentedPermissionSet = @{
		ResourceSpecificPermissions = @(
			@{
				PermissionValue = "OnlineMeeting.ReadBasic.Chat"
				PermissionType = "delegated"
			}
			@{
				PermissionValue = "ChatMessage.Read.Chat"
				PermissionType = "application"
			}
		)
	}
}

New-MgTeamInstalledApp -TeamId $teamId -BodyParameter $params

```