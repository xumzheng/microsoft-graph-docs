---
description: "Automatically generated file. DO NOT MODIFY"
---

```csharp

var graphClient = new GraphServiceClient(requestAdapter);

var requestBody = new Microsoft.Graph.Beta.Communications.Calls.Item.MicrosoftGraphReject.RejectPostRequestBody
{
	Reason = RejectReason.None,
};
await graphClient.Communications.Calls["call-id"].MicrosoftGraphReject.PostAsync(requestBody);


```