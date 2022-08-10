---
description: "Automatically generated file. DO NOT MODIFY"
---

```csharp

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
var graphClient = new GraphServiceClient(requestAdapter);

var requestBody = new DeleteTiIndicatorsByExternalIdPostRequestBody
{
	Value = new List<>
	{
		"externalId-value1",
		"externalId-value2",
	},
};
var result = await graphClient.Security.TiIndicators.DeleteTiIndicatorsByExternalId.PostAsync(requestBody);


```