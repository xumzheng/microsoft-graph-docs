---
description: "Automatically generated file. DO NOT MODIFY"
---

```csharp

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
var graphClient = new GraphServiceClient(requestAdapter);

var requestBody = new UserFlowLanguageConfiguration-idRequestBody
{
	AdditionalData = new()
	{
		{"id", "es-ES"},
		{"isEnabled", true},
	}
};
await graphClient.Identity.B2cUserFlows["b2cIdentityUserFlow-id"].Languages["userFlowLanguageConfiguration-id"].PutAsync(requestBody);


```