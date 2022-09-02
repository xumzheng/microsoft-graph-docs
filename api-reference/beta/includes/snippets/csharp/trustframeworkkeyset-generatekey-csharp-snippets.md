---
description: "Automatically generated file. DO NOT MODIFY"
---

```csharp

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
var graphClient = new GraphServiceClient(requestAdapter);

var requestBody = new GenerateKeyPostRequestBody
{
	Use = "sig",
	Kty = "RSA",
	Nbf = 1508969811L,
	Exp = 1508969811L,
};
var result = await graphClient.TrustFramework.KeySets["trustFrameworkKeySet-id"].GenerateKey.PostAsync(requestBody);


```