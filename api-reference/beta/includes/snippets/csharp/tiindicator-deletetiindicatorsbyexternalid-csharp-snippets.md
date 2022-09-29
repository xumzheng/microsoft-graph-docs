---
description: "Automatically generated file. DO NOT MODIFY"
---

```csharp

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
var graphClient = new GraphServiceClient(requestAdapter);

var requestBody = new Microsoft.Graph.Beta.Security.TiIndicators.DeleteTiIndicatorsByExternalId.DeleteTiIndicatorsByExternalIdPostRequestBody
{
	Value = new List<string>
	{
		"externalId-value1",
		"externalId-value2",
	},
};
var result = await graphClient.Security.TiIndicators.DeleteTiIndicatorsByExternalId.PostAsync(requestBody);


```