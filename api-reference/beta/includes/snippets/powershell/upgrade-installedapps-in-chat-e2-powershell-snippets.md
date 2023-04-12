---
description: "Automatically generated file. DO NOT MODIFY"
---

```powershell

Import-Module Microsoft.Graph.Teams

$params = @{
	ConsentedPermissionSet = @{
		ResourceSpecificPermissions = @(
			@{
				PermissionValue = "OnlineMeeting.ReadBasic.Chat"
				PermissionType = "Delegated"
			}
			@{
				PermissionValue = "ChatMember.Read.Chat"
				PermissionType = "Application"
			}
		)
	}
}

Update-MgChatInstalledApp -ChatId $chatId -TeamsAppInstallationId $teamsAppInstallationId -BodyParameter $params

```