---
description: "Automatically generated file. DO NOT MODIFY"
---

```csharp

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
var graphClient = new GraphServiceClient(requestAdapter);

var requestBody = new Microsoft.Graph.Beta.Identity.B2cUserFlows.Item.Languages.Item.Language
{
	AdditionalData = new Dictionary<string, object>
	{
		{
			"id" , "es-ES"
		},
		{
			"isEnabled" , true
		},
	},
};
await graphClient.Identity.B2cUserFlows["b2cIdentityUserFlow-id"].Languages["userFlowLanguageConfiguration-id"].PutAsync(requestBody);


```