---
description: "Automatically generated file. DO NOT MODIFY"
---

```powershellv2

Import-Module Microsoft.Graph.Beta.Teams

$params = @{
	"@odata.type" = "#microsoft.graph.aadUserConversationMember"
	Roles = @(
		"owner"
	)
}

Update-MgBetaTeamChannelMember -TeamId $teamId -ChannelId $channelId -ConversationMemberId $conversationMemberId -BodyParameter $params

```