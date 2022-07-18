---
description: "Automatically generated file. DO NOT MODIFY"
---

```csharp

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
var graphClient = new GraphServiceClient(requestAdapter);

var requestBody = new DataSource
{
	@odata.type = "microsoft.graph.ediscovery.siteSource",
	AdditionalData = new()
	{
	}
};
var result = await graphClient.Compliance.Ediscovery.Cases["case-id"].SourceCollections["sourceCollection-id"].AdditionalSources.PostAsync(requestBody);


```