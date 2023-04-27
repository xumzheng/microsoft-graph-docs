---
description: "Automatically generated file. DO NOT MODIFY"
---

```powershellv2

Import-Module Microsoft.Graph.Beta.Teams

$params = @{
	body = @{
		contentType = "html"
		content = "Hello World"
	}
}

New-MgBetaTeamChannelMessageReply -TeamId $teamId -ChannelId $channelId -ChatMessageId $chatMessageId -BodyParameter $params

```