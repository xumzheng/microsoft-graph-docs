---
description: "Automatically generated file. DO NOT MODIFY"
---

```csharp

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
var graphClient = new GraphServiceClient(requestAdapter);

var requestBody = new ConfirmSafePostRequestBody
{
	RequestIds = new List<>
	{
		"5a0c76d2-cb57-4ece-9bc1-c323178f116a",
		"96609214-09ef-4f80-9d4a-ace5fceecaec",
		"05020696-4eb8-45a3-918f-8f8bb7ad6015",
	},
};
await graphClient.AuditLogs.SignIns.ConfirmSafe.PostAsync(requestBody);


```