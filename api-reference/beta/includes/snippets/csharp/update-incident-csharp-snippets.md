---
description: "Automatically generated file. DO NOT MODIFY"
---

```csharp

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
var graphClient = new GraphServiceClient(requestAdapter);

var requestBody = new Microsoft.Graph.Beta..Security.Incident
{
	Classification = AlertClassification.Truepositive,
	Determination = AlertDetermination.Multistagedattack,
	Tags = new List<string>
	{
		"Demo",
	},
};
await graphClient.Security.Incidents["incident-id"].PatchAsync(requestBody);


```