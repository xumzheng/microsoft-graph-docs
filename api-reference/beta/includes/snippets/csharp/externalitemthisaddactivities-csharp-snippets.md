---
description: "Automatically generated file. DO NOT MODIFY"
---

```csharp

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
var graphClient = new GraphServiceClient(requestAdapter);

var requestBody = new Microsoft.Graph.Beta.Connections.Item.Items.Item.AddActivities.AddActivitiesPostRequestBody
{
	Activities = new List<Microsoft.Graph.Beta.Models.ExternalConnectors.ExternalActivity>
	{
		new ExternalActivity
		{
			OdataType = "#microsoft.graph.externalConnectors.externalActivity",
			Type = Microsoft.Graph.Beta.Models.ExternalConnectors.ExternalActivityType.Viewed,
			StartDateTime = DateTimeOffset.Parse("String (timestamp)"),
		},
	},
};
var result = await graphClient.Connections["externalConnection-id"].Items["externalItem-id"].AddActivities.PostAsync(requestBody);


```