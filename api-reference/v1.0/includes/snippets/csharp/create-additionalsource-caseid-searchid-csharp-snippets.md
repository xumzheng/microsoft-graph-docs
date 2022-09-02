---
description: "Automatically generated file. DO NOT MODIFY"
---

```csharp

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
var graphClient = new GraphServiceClient(requestAdapter);

var requestBody = new Microsoft.Graph..Security.DataSource
{
	OdataType = "microsoft.graph.security.siteSource",
	AdditionalData = new Dictionary<string, object>
	{
		{
			"site" , new 
			{
				WebUrl = "https://contoso.sharepoint.com/sites/SecretSite",
			}
		},
	},
};
var result = await graphClient.Security.Cases.EdiscoveryCases["ediscoveryCase-id"].Searches["ediscoverySearch-id"].AdditionalSources.PostAsync(requestBody);


```