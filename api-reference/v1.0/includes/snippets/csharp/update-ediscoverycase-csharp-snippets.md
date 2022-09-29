---
description: "Automatically generated file. DO NOT MODIFY"
---

```csharp

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
var graphClient = new GraphServiceClient(requestAdapter);

var requestBody = new Microsoft.Graph.Models.Security.EdiscoveryCase
{
	DisplayName = "My Case 1 - Renamed",
	Description = "Updated description",
};
var result = await graphClient.Security.Cases.EdiscoveryCases["ediscoveryCase-id"].PatchAsync(requestBody);


```