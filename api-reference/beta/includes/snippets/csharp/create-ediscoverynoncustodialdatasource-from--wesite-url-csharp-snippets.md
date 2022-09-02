---
description: "Automatically generated file. DO NOT MODIFY"
---

```csharp

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
var graphClient = new GraphServiceClient(requestAdapter);

var requestBody = new Microsoft.Graph.Beta..Security.EdiscoveryNoncustodialDataSource
{
	DataSource = new DataSource
	{
		OdataType = "microsoft.graph.security.siteSource",
		AdditionalData = new Dictionary<string, object>
		{
			{
				"site" , new 
				{
					WebUrl = "https://m365x809305.sharepoint.com/sites/Design-topsecret",
				}
			},
		},
	},
};
var result = await graphClient.Security.Cases.EdiscoveryCases["ediscoveryCase-id"].NoncustodialDataSources.PostAsync(requestBody);


```