---
description: "Automatically generated file. DO NOT MODIFY"
---

```csharp

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
var graphClient = new GraphServiceClient(requestAdapter);

var requestBody = new PublishedResource
{
	DisplayName = "Demo provisioning (updated)",
};
var result = await graphClient.OnPremisesPublishingProfiles["onPremisesPublishingProfile-id"].PublishedResources["publishedResource-id"].PatchAsync(requestBody);


```