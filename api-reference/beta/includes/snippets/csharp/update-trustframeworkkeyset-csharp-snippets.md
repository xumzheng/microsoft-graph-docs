---
description: "Automatically generated file. DO NOT MODIFY"
---

```csharp

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
var graphClient = new GraphServiceClient(requestAdapter);

var requestBody = new TrustFrameworkKeySet-idRequestBody
{
	AdditionalData = new()
	{
		{"keys", new List<Object>
		{
		}
	}
};
await graphClient.TrustFramework.KeySets["trustFrameworkKeySet-id"].PutAsync(requestBody);


```