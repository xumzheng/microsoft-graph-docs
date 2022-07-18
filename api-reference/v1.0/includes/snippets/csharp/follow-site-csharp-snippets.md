---
description: "Automatically generated file. DO NOT MODIFY"
---

```csharp

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
var graphClient = new GraphServiceClient(requestAdapter);

var requestBody = new Site-idRequestBody
{
	AdditionalData = new()
	{
		{"value", new List<Object>
		{
		}
	}
};
await graphClient.Users["user-id"].FollowedSites["site-id"].PostAsync(requestBody);


```