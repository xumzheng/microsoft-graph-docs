---
description: "Automatically generated file. DO NOT MODIFY"
---

```csharp

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
var graphClient = new GraphServiceClient(requestAdapter);

var requestBody = new Microsoft.Graph.Beta..Ediscovery.SourceCollection
{
	DisplayName = "Quarterly Financials search",
};
await graphClient.Compliance.Ediscovery.Cases["case-id"].SourceCollections["sourceCollection-id"].PatchAsync(requestBody);


```