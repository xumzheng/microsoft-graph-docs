---
description: "Automatically generated file. DO NOT MODIFY"
---

```csharp

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
var graphClient = new GraphServiceClient(requestAdapter);

var requestBody = new UnfavoritePostRequestBody
{
	MessageIds = new List<>
	{
		"MC172851",
		"MC167983",
	},
};
var result = await graphClient.Admin.ServiceAnnouncement.Messages.Unfavorite.PostAsync(requestBody);


```