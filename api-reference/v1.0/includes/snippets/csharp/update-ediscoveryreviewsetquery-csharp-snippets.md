---
description: "Automatically generated file. DO NOT MODIFY"
---

```csharp

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
var graphClient = new GraphServiceClient(requestAdapter);

var requestBody = new Microsoft.Graph.Models.Security.EdiscoveryReviewSetQuery
{
	DisplayName = "My Query 1 (update)",
	ContentQuery = "(Author=\"edisons\")",
};
await graphClient.Security.Cases.EdiscoveryCases["ediscoveryCase-id"].ReviewSets["ediscoveryReviewSet-id"].Queries["ediscoveryReviewSetQuery-id"].PatchAsync(requestBody);


```