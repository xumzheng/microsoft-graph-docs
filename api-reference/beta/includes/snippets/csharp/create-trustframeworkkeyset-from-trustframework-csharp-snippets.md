---
description: "Automatically generated file. DO NOT MODIFY"
---

```csharp

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
var graphClient = new GraphServiceClient(requestAdapter);

var requestBody = new TrustFrameworkKeySet
{
	Id = "keyset1",
	Keys = new List<TrustFrameworkKey>
	{
		new TrustFrameworkKey
		{
			K = "k-value",
			X5c = new List<string>
			{
				"x5c-value",
			},
			X5t = "x5t-value",
			Kty = "kty-value",
			Use = "use-value",
			Exp = 99L,
			Nbf = 99L,
			Kid = "kid-value",
			E = "e-value",
			N = "n-value",
			D = "d-value",
			P = "p-value",
			Q = "q-value",
			Dp = "dp-value",
			Dq = "dq-value",
			Qi = "qi-value",
		},
	},
};
var result = await graphClient.TrustFramework.KeySets.PostAsync(requestBody);


```