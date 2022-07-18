---
description: "Automatically generated file. DO NOT MODIFY"
---

```csharp

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
var graphClient = new GraphServiceClient(requestAdapter);

var requestBody = new ValueRequestBody
{
	Value = new List<Object>
	{
		new 
		{
			AdditionalData = new()
			{
				{"id", "c6fb948b-89c5-3bba-a2cd-a9d9a1e430e4"},
				{"additionalInformation", "mytest"},
			}
		},
		new 
		{
			AdditionalData = new()
			{
				{"id", "e58c072b-c9bb-a5c4-34ce-eb69af44fb1e"},
				{"additionalInformation", "test again"},
			}
		},
	}
};
var result = await graphClient.Security.TiIndicators.UpdateTiIndicators.PostAsync(requestBody);


```