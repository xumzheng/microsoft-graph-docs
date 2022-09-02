---
description: "Automatically generated file. DO NOT MODIFY"
---

```csharp

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
var graphClient = new GraphServiceClient(requestAdapter);

var requestBody = new Microsoft.Graph.Models.Security.EdiscoverySearch
{
	DisplayName = "Teams search",
};
await graphClient.Security.Cases.EdiscoveryCases["ediscoveryCase-id"].Searches["ediscoverySearch-id"].PatchAsync(requestBody);


```