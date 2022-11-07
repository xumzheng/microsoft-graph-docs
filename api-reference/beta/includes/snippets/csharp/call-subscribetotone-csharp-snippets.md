---
description: "Automatically generated file. DO NOT MODIFY"
---

```csharp

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
var graphClient = new GraphServiceClient(requestAdapter);

var requestBody = new Microsoft.Graph.Beta.Communications.Calls.Item.SubscribeToTone.SubscribeToTonePostRequestBody
{
	ClientContext = "fd1c7836-4d84-4e24-b6aa-23188688cc54",
};
var result = await graphClient.Communications.Calls["call-id"].SubscribeToTone.PostAsync(requestBody);


```