---
description: "Automatically generated file. DO NOT MODIFY"
---

```powershellv2

Import-Module Microsoft.Graph.Beta.Teams

$params = @{
	DisplayName = "UpdateChannelModeration"
	Description = "Update channel moderation."
	ModerationSettings = @{
		UserNewMessageRestriction = "moderators"
		ReplyRestriction = "everyone"
		AllowNewMessageFromBots = $true
		AllowNewMessageFromConnectors = $true
	}
}

Update-MgBetaTeamChannel -TeamId $teamId -ChannelId $channelId -BodyParameter $params

```