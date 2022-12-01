---
description: "Automatically generated file. DO NOT MODIFY"
---

```csharp

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
var graphClient = new GraphServiceClient(requestAdapter);

var requestBody = new Microsoft.Graph.Beta.IdentityGovernance.LifecycleWorkflows.Workflows.Item.Activate.ActivatePostRequestBody
{
	Subjects = new List<User>
	{
		new User
		{
			Id = "df744d9e-2148-4922-88a8-633896c1e929",
		},
	},
};
await graphClient.IdentityGovernance.LifecycleWorkflows.Workflows["workflow-id"].Activate.PostAsync(requestBody);


```