---
description: "Automatically generated file. DO NOT MODIFY"
---

```csharp

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
var graphClient = new GraphServiceClient(requestAdapter);

var requestBody = new UploadSecretPostRequestBody
{
	Use = "use-value",
	K = "application-secret-to-be-uploaded",
	Nbf = 1508969811L,
	Exp = 1508973711L,
};
var result = await graphClient.TrustFramework.KeySets["trustFrameworkKeySet-id"].UploadSecret.PostAsync(requestBody);


```