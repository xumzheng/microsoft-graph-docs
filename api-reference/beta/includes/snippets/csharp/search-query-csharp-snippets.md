---
description: "Automatically generated file. DO NOT MODIFY"
---

```csharp

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
var graphClient = new GraphServiceClient(requestAdapter);

var requestBody = new QueryPostRequestBody
{
	Requests = new List<SearchRequest>
	{
		new SearchRequest
		{
			AdditionalData = new Dictionary<string, object>
			{
				{
					"entityTypes" , new List<>
					{
						"externalItem",
					}
				},
				{
					"contentSources" , new List<>
					{
						"/external/connections/connectionfriendlyname",
					}
				},
				{
					"query" , new 
					{
						QueryString = "contoso product",
					}
				},
				{
					"from" , 0
				},
				{
					"size" , 25
				},
				{
					"fields" , new List<>
					{
						"title",
						"description",
					}
				},
			},
		},
	},
};
var result = await graphClient.Search.Query.PostAsync(requestBody);


```