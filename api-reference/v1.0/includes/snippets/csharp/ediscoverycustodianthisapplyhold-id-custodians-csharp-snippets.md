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
		"7f697316-43ed-48e1-977f-261be050db93",
		"b26888b3-e1f5-47c5-bdf2-33d1b90cb2e8",
	},
};
await graphClient.Security.Cases.EdiscoveryCases["ediscoveryCase-id"].Custodians.ApplyHold.PostAsync(requestBody);


```