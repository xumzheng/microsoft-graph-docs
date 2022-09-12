---
description: "Automatically generated file. DO NOT MODIFY"
---

```csharp

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
var graphClient = new GraphServiceClient(requestAdapter);

var requestBody = new Microsoft.Graph.Beta.Models.Security.Incident
{
	Classification = Microsoft.Graph.Beta.Models.Security.AlertClassification.TruePositive,
	Determination = Microsoft.Graph.Beta.Models.Security.AlertDetermination.MultiStagedAttack,
	Tags = new List<string>
	{
		"Demo",
	},
};
await graphClient.Security.Incidents["incident-id"].PatchAsync(requestBody);


```