---
description: "Automatically generated file. DO NOT MODIFY"
---

```csharp

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
var graphClient = new GraphServiceClient(requestAdapter);

var requestBody = new SynchronizationJob
{
	TemplateId = "BoxOutDelta",
};
var result = await graphClient.ServicePrincipals["servicePrincipal-id"].Synchronization.Jobs.PostAsync(requestBody);


```