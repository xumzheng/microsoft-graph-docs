---
description: "Automatically generated file. DO NOT MODIFY"
---

```csharp

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
var graphClient = new GraphServiceClient(requestAdapter);

var requestBody = new Group
{
	Description = "Contoso Life v2.0",
	DisplayName = "Contoso Life Renewed",
};
var result = await graphClient.Groups["group-id"].PatchAsync(requestBody);


```