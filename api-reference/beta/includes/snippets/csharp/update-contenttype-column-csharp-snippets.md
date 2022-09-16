---
description: "Automatically generated file. DO NOT MODIFY"
---

```csharp

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
var graphClient = new GraphServiceClient(requestAdapter);

var requestBody = new ColumnDefinition
{
	Required = true,
	Hidden = false,
	PropagateChanges = false,
};
await graphClient.Sites["site-id"].ContentTypes["contentType-id"].Columns["columnDefinition-id"].PatchAsync(requestBody);


```