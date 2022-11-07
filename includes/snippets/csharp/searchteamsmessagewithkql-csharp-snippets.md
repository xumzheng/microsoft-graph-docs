---
description: "Automatically generated file. DO NOT MODIFY"
---

```csharp

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
var graphClient = new GraphServiceClient(requestAdapter);

var requestBody = new Microsoft.Graph.Search.Query.QueryPostRequestBody
{
	Requests = new List<SearchRequest>
	{
		new SearchRequest
		{
			EntityTypes = new List<EntityType?>
			{
				EntityType.Event,
			},
			Query = new SearchQuery
			{
				QueryString = "contoso from:bob to:alice sent>2022-07-14",
			},
			From = 0,
			Size = 15,
			EnableTopResults = true,
		},
	},
};
var result = await graphClient.Search.Query.PostAsync(requestBody);


```