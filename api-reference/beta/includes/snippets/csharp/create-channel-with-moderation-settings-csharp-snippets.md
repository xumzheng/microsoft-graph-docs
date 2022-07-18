---
description: "Automatically generated file. DO NOT MODIFY"
---

```csharp

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
var graphClient = new GraphServiceClient(requestAdapter);

var requestBody = new Channel
{
	DisplayName = "TestChannelModeration",
	Description = "Test channel moderation.",
	MembershipType = "standard",
	ModerationSettings = new ChannelModerationSettings
	{
		UserNewMessageRestriction = "everyoneExceptGuests",
		ReplyRestriction = "everyone",
		AllowNewMessageFromBots = true,
		AllowNewMessageFromConnectors = true,
	},
};
var result = await graphClient.Teams["team-id"].Channels.PostAsync(requestBody);


```