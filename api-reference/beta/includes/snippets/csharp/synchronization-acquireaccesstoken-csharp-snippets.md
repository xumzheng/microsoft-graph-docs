---
description: "Automatically generated file. DO NOT MODIFY"
---

```csharp

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
var graphClient = new GraphServiceClient(requestAdapter);

var requestBody = new AcquireAccessTokenPostRequestBody
{
	Credentials = new List<SynchronizationSecretKeyStringValuePair>
	{
		new SynchronizationSecretKeyStringValuePair
		{
			OdataType = "microsoft.graph.synchronizationSecretKeyStringValuePair",
		},
	},
};
await graphClient.Applications["application-id"].Synchronization.AcquireAccessToken.PostAsync(requestBody);


```