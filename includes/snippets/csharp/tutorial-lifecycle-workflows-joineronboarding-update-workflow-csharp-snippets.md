---
description: "Automatically generated file. DO NOT MODIFY"
---

```csharp

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
var graphClient = new GraphServiceClient(requestAdapter);

var requestBody = new Microsoft.Graph.Beta.Models.IdentityGovernance.Workflow
{
	IsEnabled = true,
	IsSchedulingEnabled = true,
};
var result = await graphClient.IdentityGovernance.LifecycleWorkflows.Workflows["workflow-id"].PatchAsync(requestBody);


```