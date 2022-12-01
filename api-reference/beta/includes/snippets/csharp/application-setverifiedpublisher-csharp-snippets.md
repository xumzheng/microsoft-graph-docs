---
description: "Automatically generated file. DO NOT MODIFY"
---

```csharp

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
var graphClient = new GraphServiceClient(requestAdapter);

var requestBody = new Microsoft.Graph.Beta.Applications.Item.SetVerifiedPublisher.SetVerifiedPublisherPostRequestBody
{
	VerifiedPublisherId = "1234567",
};
await graphClient.Applications["application-id"].SetVerifiedPublisher.PostAsync(requestBody);


```