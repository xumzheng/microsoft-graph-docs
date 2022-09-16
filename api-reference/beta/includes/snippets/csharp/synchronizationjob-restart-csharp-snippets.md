---
description: "Automatically generated file. DO NOT MODIFY"
---

```csharp

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
var graphClient = new GraphServiceClient(requestAdapter);

var requestBody = new Microsoft.Graph.Beta.ServicePrincipals.Item.Synchronization.Jobs.Item.Restart.RestartPostRequestBody
{
	Criteria = new SynchronizationJobRestartCriteria
	{
		ResetScope = SynchronizationJobRestartScope.Watermark | SynchronizationJobRestartScope.Escrows | SynchronizationJobRestartScope.QuarantineState,
	},
};
await graphClient.ServicePrincipals["servicePrincipal-id"].Synchronization.Jobs["synchronizationJob-id"].Restart.PostAsync(requestBody, (requestConfiguration) =>
{
	requestConfiguration.Headers.Add("Authorization", "Bearer <token>");
});


```