---
description: "Automatically generated file. DO NOT MODIFY"
---

```csharp

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
var graphClient = new GraphServiceClient(requestAdapter);

var requestBody = new Microsoft.Graph.Applications.Item.AddKey.AddKeyPostRequestBody
{
	KeyCredential = new KeyCredential
	{
		Type = "AsymmetricX509Cert",
		Usage = "Verify",
		Key = Convert.FromBase64String("MIIDYDCCAki..."),
	},
	PasswordCredential = null,
	Proof = "eyJ0eXAiOiJ...",
};
var result = await graphClient.Applications["application-id"].AddKey.PostAsync(requestBody);


```