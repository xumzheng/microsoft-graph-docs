---
description: "Automatically generated file. DO NOT MODIFY"
---

```csharp

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
var graphClient = new GraphServiceClient(requestAdapter);

var requestBody = new SchemaPostRequestBody
{
	AdditionalData = new Dictionary<string, object>
	{
		{
			"baseType" , "microsoft.graph.externalItem"
		},
		{
			"properties" , new List<>
			{
				new 
				{
					Name = "ticketTitle",
					Type = "string",
					IsSearchable = "true",
					IsRetrievable = "true",
					Labels = new List<>
					{
						"title",
					},
				},
				new 
				{
					Name = "priority",
					Type = "string",
					IsQueryable = "true",
					IsRetrievable = "true",
					IsSearchable = "false",
				},
				new 
				{
					Name = "assignee",
					Type = "string",
					IsRetrievable = "true",
				},
			}
		},
	},
};
await graphClient.External.Connections["externalConnection-id"].Schema.PostAsync(requestBody);


```