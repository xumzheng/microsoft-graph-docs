---
description: "Automatically generated file. DO NOT MODIFY"
---

```csharp

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
var graphClient = new GraphServiceClient(requestAdapter);

var requestBody = new KeySet
{
	AdditionalData = new Dictionary<string, object>
	{
		{
			"keys" , new List<>
			{
				new 
				{
					K = "k-value",
					X5c = new List<>
					{
						"x5c-value",
					},
					X5t = "x5t-value",
					Kty = "kty-value",
					Use = "use-value",
					Exp = 99,
					Nbf = 99,
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
			}
		},
	},
};
await graphClient.TrustFramework.KeySets["trustFrameworkKeySet-id"].PutAsync(requestBody);


```