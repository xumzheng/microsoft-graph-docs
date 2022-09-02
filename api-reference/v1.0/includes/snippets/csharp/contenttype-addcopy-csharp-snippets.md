---
description: "Automatically generated file. DO NOT MODIFY"
---

```csharp

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
var graphClient = new GraphServiceClient(requestAdapter);

var requestBody = new AddCopyPostRequestBody
{
	ContentType = "https://graph.microsoft.com/v1.0/sites/{site-id}/contentTypes/0x0101",
};
var result = await graphClient.Sites["site-id"].Lists["list-id"].ContentTypes.AddCopy.PostAsync(requestBody);


```