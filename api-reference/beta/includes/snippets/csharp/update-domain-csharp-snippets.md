---
description: "Automatically generated file. DO NOT MODIFY"
---

```csharp

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
var graphClient = new GraphServiceClient(requestAdapter);

var requestBody = new Domain
{
	IsDefault = true,
	SupportedServices = new List<>
	{
		"Email",
		"OfficeCommunicationsOnline",
	},
};
await graphClient.Domains["domain-id"].PatchAsync(requestBody);


```