---
description: "Automatically generated file. DO NOT MODIFY"
---

```csharp

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
var graphClient = new GraphServiceClient(requestAdapter);

var requestBody = new Microsoft.Graph.Beta.Models.Ediscovery.ReviewSetQuery
{
	DisplayName = "My Query 1 - Renamed",
};
await graphClient.Compliance.Ediscovery.Cases["case-id"].ReviewSets["reviewSet-id"].Queries["reviewSetQuery-id"].PatchAsync(requestBody);


```