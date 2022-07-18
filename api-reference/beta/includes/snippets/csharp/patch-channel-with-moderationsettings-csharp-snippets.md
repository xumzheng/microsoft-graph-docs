---
description: "Automatically generated file. DO NOT MODIFY"
---

```csharp

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
var graphClient = new GraphServiceClient(requestAdapter);

var requestBody = new Channel
{
	DisplayName = "UpdateChannelModeration",
	Description = "Update channel moderation.",
	ModerationSettings = new ChannelModerationSettings
	{
		UserNewMessageRestriction = "moderators",
		ReplyRestriction = "everyone",
		AllowNewMessageFromBots = true,
		AllowNewMessageFromConnectors = true,
	},
};
await graphClient.Teams["team-id"].Channels["channel-id"].PatchAsync(requestBody);


```