---
description: "Automatically generated file. DO NOT MODIFY"
---

```csharp

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
var graphClient = new GraphServiceClient(requestAdapter);

var requestBody = new Extension
{
	AdditionalData = new Dictionary<string, object>
	{
		{
			"theme" , "light"
		},
		{
			"color" , "yellow"
		},
		{
			"lang" , "Swahili"
		},
	},
};
var result = await graphClient.Me.Extensions["extension-id"].PatchAsync(requestBody);


```