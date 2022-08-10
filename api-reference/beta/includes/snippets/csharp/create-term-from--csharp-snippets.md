---
description: "Automatically generated file. DO NOT MODIFY"
---

```csharp

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
var graphClient = new GraphServiceClient(requestAdapter);

var requestBody = new Term
{
	Labels = new List<LocalizedLabel>
	{
		new LocalizedLabel
		{
			LanguageTag = "en-US",
			Name = "Car",
			IsDefault = true,
		},
	},
};
var result = await graphClient.TermStore.Sets["set-id"].Children.PostAsync(requestBody);


```