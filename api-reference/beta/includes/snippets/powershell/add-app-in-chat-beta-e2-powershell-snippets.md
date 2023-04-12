---
description: "Automatically generated file. DO NOT MODIFY"
---

```powershell

Import-Module Microsoft.Graph.Teams

$params = @{
	"TeamsApp@odata.bind" = "https://graph.microsoft.com/beta/appCatalogs/teamsApps/2b524e28-95ce-4c9b-9773-4a5bd6ec1770"
	ConsentedPermissionSet = @{
		ResourceSpecificPermissions = @(
			@{
				PermissionValue = "OnlineMeeting.ReadBasic.Chat"
				PermissionType = "Delegated"
			}
			@{
				PermissionValue = "OnlineMeetingIncomingAudio.Detect.Chat"
				PermissionType = "Delegated"
			}
			@{
				PermissionValue = "ChatMember.Read.Chat"
				PermissionType = "Application"
			}
			@{
				PermissionValue = "ChatMessage.Read.Chat"
				PermissionType = "Application"
			}
		)
	}
}

New-MgChatInstalledApp -ChatId $chatId -BodyParameter $params

```