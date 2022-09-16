---
description: "Automatically generated file. DO NOT MODIFY"
---

```csharp

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
var graphClient = new GraphServiceClient(requestAdapter);

var requestBody = new ContentType
{
	Name = "docSet",
	Description = "custom docset",
	Base = new ContentType
	{
		Name = "Document Set",
		Id = "0x0120D520",
	},
	Group = "Document Set Content Types",
};
var result = await graphClient.Sites["site-id"].ContentTypes.PostAsync(requestBody);


```