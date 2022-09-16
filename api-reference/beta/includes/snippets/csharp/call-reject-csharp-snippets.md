---
description: "Automatically generated file. DO NOT MODIFY"
---

```csharp

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
var graphClient = new GraphServiceClient(requestAdapter);

var requestBody = new Microsoft.Graph.Beta.Communications.Calls.Item.Reject.RejectPostRequestBody
{
	Reason = RejectReason.Busy,
};
await graphClient.Communications.Calls["call-id"].Reject.PostAsync(requestBody);


```