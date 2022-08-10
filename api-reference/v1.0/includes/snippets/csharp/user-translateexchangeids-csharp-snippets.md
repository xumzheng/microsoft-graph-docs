---
description: "Automatically generated file. DO NOT MODIFY"
---

```csharp

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
var graphClient = new GraphServiceClient(requestAdapter);

var requestBody = new TranslateExchangeIdsPostRequestBody
{
	InputIds = new List<>
	{
		"{rest-formatted-id-1}",
		"{rest-formatted-id-2}",
	},
	SourceIdType = ExchangeIdFormat.Restid,
	TargetIdType = ExchangeIdFormat.Restimmutableentryid,
};
var result = await graphClient.Me.TranslateExchangeIds.PostAsync(requestBody);


```