---
description: "Automatically generated file. DO NOT MODIFY"
---

```csharp

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
var graphClient = new GraphServiceClient(requestAdapter);

var requestBody = new ApplyHoldPostRequestBody
{
	Ids = new List<>
	{
		"39333641443238353535383731453339",
		"46333131344239353834433430454335",
	},
};
await graphClient.Security.Cases.EdiscoveryCases["ediscoveryCase-id"].NoncustodialDataSources.ApplyHold.PostAsync(requestBody);


```