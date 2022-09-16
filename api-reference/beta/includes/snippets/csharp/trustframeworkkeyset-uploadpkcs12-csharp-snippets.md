---
description: "Automatically generated file. DO NOT MODIFY"
---

```csharp

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
var graphClient = new GraphServiceClient(requestAdapter);

var requestBody = new Microsoft.Graph.Beta.TrustFramework.KeySets.Item.UploadPkcs12.UploadPkcs12PostRequestBody
{
	Key = "Base64-encoded-pfx-content",
	Password = "password-value",
};
var result = await graphClient.TrustFramework.KeySets["trustFrameworkKeySet-id"].UploadPkcs12.PostAsync(requestBody);


```