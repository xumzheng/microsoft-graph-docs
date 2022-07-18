---
description: "Automatically generated file. DO NOT MODIFY"
---

```csharp

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
var graphClient = new GraphServiceClient(requestAdapter);

var requestBody = new EdiscoveryNoncustodialDataSource
{
	DataSource = new 
	{
		@odata.type = "microsoft.graph.security.siteSource",
		AdditionalData = new()
		{
		}
	},
};
var result = await graphClient.Security.Cases.EdiscoveryCases["ediscoveryCase-id"].NoncustodialDataSources.PostAsync(requestBody);


```