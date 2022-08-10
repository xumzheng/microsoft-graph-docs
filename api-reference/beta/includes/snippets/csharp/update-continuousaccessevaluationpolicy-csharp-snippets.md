---
description: "Automatically generated file. DO NOT MODIFY"
---

```csharp

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
var graphClient = new GraphServiceClient(requestAdapter);

var requestBody = new ContinuousAccessEvaluationPolicy
{
	OdataType = "#microsoft.graph.continuousAccessEvaluationPolicy",
	Migrate = true,
};
await graphClient.Identity.ContinuousAccessEvaluationPolicy.PatchAsync(requestBody);


```