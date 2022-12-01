---
description: "Automatically generated file. DO NOT MODIFY"
---

```csharp

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
var graphClient = new GraphServiceClient(requestAdapter);

var requestBody = new ListItem
{
	Fields = new FieldValueSet
	{
		AdditionalData = new Dictionary<string, object>
		{
			{
				"Title" , "Widget"
			},
			{
				"Color" , "Purple"
			},
			{
				"Weight" , 32
			},
		},
	},
};
var result = await graphClient.Sites["site-id"].Lists["list-id"].Items.PostAsync(requestBody);


```