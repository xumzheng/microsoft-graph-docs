---
description: "Automatically generated file. DO NOT MODIFY"
---

```csharp

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
var graphClient = new GraphServiceClient(requestAdapter);

var requestBody = new RequestsRequestBody
{
	Requests = new List<SearchRequest>
	{
		new SearchRequest
		{
			AdditionalData = new()
			{
				{"entityTypes", new List<String>
				{
					"externalItem",
				}
				{"contentSources", new List<String>
				{
					"/external/connections/connectionfriendlyname",
				}
				{"from", },
				{"size", },
				{"fields", new List<String>
				{
					"title",
					"description",
				}
			}
		},
	}
};
var result = await graphClient.Search.Query.PostAsync(requestBody);


```