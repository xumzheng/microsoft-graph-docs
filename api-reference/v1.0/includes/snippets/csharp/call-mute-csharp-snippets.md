---
description: "Automatically generated file. DO NOT MODIFY"
---

```csharp

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
var graphClient = new GraphServiceClient(requestAdapter);

var requestBody = new Microsoft.Graph.Communications.Calls.Item.Mute.MutePostRequestBody
{
	ClientContext = "clientContext-value",
};
var result = await graphClient.Communications.Calls["call-id"].Mute.PostAsync(requestBody);


```