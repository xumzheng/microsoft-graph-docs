---
description: "Automatically generated file. DO NOT MODIFY"
---

```csharp

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
var graphClient = new GraphServiceClient(requestAdapter);

var requestBody = new FieldValueSet
{
	AdditionalData = new Dictionary<string, object>
	{
		{
			"Color" , "Fuchsia"
		},
		{
			"Quantity" , 934
		},
	},
};
await graphClient.Sites["site-id"].Lists["list-id"].Items["listItem-id"].Fields.PatchAsync(requestBody);


```