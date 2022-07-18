---
description: "Automatically generated file. DO NOT MODIFY"
---

```csharp

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
var graphClient = new GraphServiceClient(requestAdapter);

var requestBody = new Case
{
	DisplayName = "My Case 1 - Renamed",
	Description = "Updated description",
	ExternalId = "Updated externalId",
};
await graphClient.Compliance.Ediscovery.Cases["case-id"].PatchAsync(requestBody);


```