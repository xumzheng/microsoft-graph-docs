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
		{
			"discoverySettings" , new 
			{
				ShowInTeamsSearchAndSuggestions = true,
			}
		},
	},
};
await graphClient.Groups["group-id"].Team.PutAsync(requestBody);


```