---
description: "Automatically generated file. DO NOT MODIFY"
---

```csharp

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
var graphClient = new GraphServiceClient(requestAdapter);

var requestBody = new SynchronizationTemplate-idRequestBody
{
	AdditionalData = new()
	{
		{"id", "Slack"},
		{"applicationId", "{id}"},
		{"factoryTag", "CustomSCIM"},
	}
};
await graphClient.Applications["application-id"].Synchronization.Templates["synchronizationTemplate-id"].PutAsync(requestBody, (requestConfiguration) =>
{
	requestConfiguration.Headers.Add("Authorization", "Bearer <token>");
});


```