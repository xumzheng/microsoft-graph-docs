---
description: "Automatically generated file. DO NOT MODIFY"
---

```csharp

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
var graphClient = new GraphServiceClient(requestAdapter);

var requestBody = new CancelMediaProcessingPostRequestBody
{
	ClientContext = "clientContext-value",
};
var result = await graphClient.Communications.Calls["call-id"].CancelMediaProcessing.PostAsync(requestBody);


```