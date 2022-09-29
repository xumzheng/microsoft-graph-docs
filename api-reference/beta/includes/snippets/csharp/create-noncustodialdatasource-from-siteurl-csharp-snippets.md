---
description: "Automatically generated file. DO NOT MODIFY"
---

```csharp

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
var graphClient = new GraphServiceClient(requestAdapter);

var requestBody = new Microsoft.Graph.Beta.Models.Ediscovery.NoncustodialDataSource
{
	ApplyHoldToSource = false,
	DataSource = new Microsoft.Graph.Beta.Models.Ediscovery.DataSource
	{
		OdataType = "microsoft.graph.ediscovery.siteSource",
		AdditionalData = new Dictionary<string, object>
		{
			{
				"site" , new 
				{
					WebUrl = "https://contoso.sharepoint.com/sites/SecretSite",
				}
			},
		},
	},
};
var result = await graphClient.Compliance.Ediscovery.Cases["case-id"].NoncustodialDataSources.PostAsync(requestBody);


```