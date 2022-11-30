---
description: "Automatically generated file. DO NOT MODIFY"
---

```powershellv2

Import-Module Microsoft.Graph.Beta.Teams

$params = @{
	DisplayName = "TestChannelModeration"
	Description = "Test channel moderation."
	MembershipType = "standard"
	ModerationSettings = @{
		UserNewMessageRestriction = "everyoneExceptGuests"
		ReplyRestriction = "everyone"
		AllowNewMessageFromBots = $true
		AllowNewMessageFromConnectors = $true
	}
}

New-MgBetaTeamChannel -TeamId $teamId -BodyParameter $params

```