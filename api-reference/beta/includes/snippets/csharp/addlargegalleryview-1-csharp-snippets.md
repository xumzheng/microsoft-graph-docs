---
description: "Automatically generated file. DO NOT MODIFY"
---

```csharp

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
var graphClient = new GraphServiceClient(requestAdapter);

var requestBody = new Microsoft.Graph.Beta.Communications.Calls.Item.AddLargeGalleryView.AddLargeGalleryViewPostRequestBody
{
	ClientContext = "785f4929-92ca-497b-863f-c778c77c9758",
};
var result = await graphClient.Communications.Calls["call-id"].AddLargeGalleryView.PostAsync(requestBody);


```