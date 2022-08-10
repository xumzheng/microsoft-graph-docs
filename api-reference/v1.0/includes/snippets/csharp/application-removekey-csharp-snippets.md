---
description: "Automatically generated file. DO NOT MODIFY"
---

```csharp

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
var graphClient = new GraphServiceClient(requestAdapter);

var requestBody = new RemoveKeyPostRequestBody
{
	KeyId = "f0b0b335-1d71-4883-8f98-567911bfdca6",
	Proof = "eyJ0eXAiOiJ...",
};
await graphClient.Applications["application-id"].RemoveKey.PostAsync(requestBody);


```