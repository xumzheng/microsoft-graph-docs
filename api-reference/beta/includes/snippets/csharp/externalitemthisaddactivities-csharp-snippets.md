---
description: "Automatically generated file. DO NOT MODIFY"
---

```csharp

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
var graphClient = new GraphServiceClient(requestAdapter);

var requestBody = new AddActivitiesPostRequestBody
{
	Activities = new List<ExternalActivity>
	{
		new ExternalActivity
		{
			OdataType = "#microsoft.graph.externalConnectors.externalActivity",
			Type = ExternalActivityType.String,
			StartDateTime = DateTimeOffset.Parse("String (timestamp)"),
		},
	},
};
var result = await graphClient.Connections["externalConnection-id"].Items["externalItem-id"].AddActivities.PostAsync(requestBody);


```