---
description: "Automatically generated file. DO NOT MODIFY"
---

```csharp

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
var graphClient = new GraphServiceClient(requestAdapter);

var requestBody = new Microsoft.Graph..TermStore.Store
{
	DefaultLanguageTag = "en-US",
};
await graphClient.Sites["site-id"].TermStore.PatchAsync(requestBody);


```