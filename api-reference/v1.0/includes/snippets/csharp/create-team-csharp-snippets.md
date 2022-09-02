---
description: "Automatically generated file. DO NOT MODIFY"
---

```csharp

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
var graphClient = new GraphServiceClient(requestAdapter);

var requestBody = new TeamPostRequestBody
{
	AdditionalData = new Dictionary<string, object>
	{
		{
			"memberSettings" , new 
			{
				AllowCreatePrivateChannels = true,
				AllowCreateUpdateChannels = true,
			}
		},
		{
			"messagingSettings" , new 
			{
				AllowUserEditMessages = true,
				AllowUserDeleteMessages = true,
			}
		},
		{
			"funSettings" , new 
			{
				AllowGiphy = true,
				GiphyContentRating = "strict",
			}
		},
	},
};
await graphClient.Groups["group-id"].Team.PutAsync(requestBody);


```