---
description: "Automatically generated file. DO NOT MODIFY"
---

```csharp

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
var graphClient = new GraphServiceClient(requestAdapter);

var requestBody = new NoncustodialDataSource
{
	ApplyHoldToSource = false,
	DataSource = new 
	{
		@odata.type = "microsoft.graph.ediscovery.siteSource",
		AdditionalData = new()
		{
		}
	},
};
var result = await graphClient.Compliance.Ediscovery.Cases["case-id"].NoncustodialDataSources.PostAsync(requestBody);


```