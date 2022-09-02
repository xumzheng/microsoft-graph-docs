---
description: "Automatically generated file. DO NOT MODIFY"
---

```csharp

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
var graphClient = new GraphServiceClient(requestAdapter);

var requestBody = new Microsoft.Graph.Beta..ExternalConnectors.Schema
{
	BaseType = "microsoft.graph.externalItem",
	Properties = new List<Microsoft.Graph.Beta..ExternalConnectors.Property>
	{
		new Property
		{
			Name = "ticketTitle",
			Type = PropertyType.String,
			IsSearchable = true,
			IsRetrievable = true,
			Labels = new List<>
			{
				Label.Title,
			},
		},
		new Property
		{
			Name = "priority",
			Type = PropertyType.String,
			IsQueryable = true,
			IsRetrievable = true,
			IsSearchable = false,
		},
		new Property
		{
			Name = "assignee",
			Type = PropertyType.String,
			IsRetrievable = true,
		},
	},
};
await graphClient.External.Connections["externalConnection-id"].Schema.PatchAsync(requestBody);


```