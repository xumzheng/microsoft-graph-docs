---
description: "Automatically generated file. DO NOT MODIFY"
---

```csharp

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
var graphClient = new GraphServiceClient(requestAdapter);

var requestBody = new Microsoft.Graph.Beta..Search.Bookmark
{
	Description = "Book a fancy vacation in Tuscany or browse museums in Florence.",
};
await graphClient.Search.Bookmarks["bookmark-id"].PatchAsync(requestBody);


```