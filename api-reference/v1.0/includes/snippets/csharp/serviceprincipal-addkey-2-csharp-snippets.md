---
description: "Automatically generated file. DO NOT MODIFY"
---

```csharp

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
var graphClient = new GraphServiceClient(requestAdapter);

var requestBody = new KeyCredentialPostRequestBody
{
	KeyCredential = new KeyCredential
	{
		Type = "X509CertAndPassword",
		Usage = "Sign",
		Key = Convert.FromBase64String("MIIDYDCCAki..."),
	},
	PasswordCredential = new PasswordCredential
	{
		SecretText = "MKTr0w1...",
	},
	Proof = "eyJ0eXAiOiJ...",
};
var result = await graphClient.ServicePrincipals["servicePrincipal-id"].AddKey.PostAsync(requestBody);


```