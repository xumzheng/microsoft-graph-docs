---
description: "Automatically generated file. DO NOT MODIFY"
---

```csharp

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
var graphClient = new GraphServiceClient(requestAdapter);

var requestBody = new Schema
{
	BaseType = "microsoft.graph.externalItem",
	Properties = new List<Property>
	{
		new Property
		{
			Name = "ticketTitle",
			Type = "string",
			IsSearchable = "true",
			IsRetrievable = "true",
			Labels = new List<Label>
			{
				"title",
			}
		},
		new Property
		{
			Name = "priority",
			Type = "string",
			IsQueryable = "true",
			IsRetrievable = "true",
			IsSearchable = "false",
		},
		new Property
		{
			Name = "assignee",
			Type = "string",
			IsRetrievable = "true",
		},
	}
};
await graphClient.External.Connections["externalConnection-id"].Schema.PatchAsync(requestBody);


```