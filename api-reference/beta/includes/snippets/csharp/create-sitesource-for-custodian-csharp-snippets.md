---
description: "Automatically generated file. DO NOT MODIFY"
---

```csharp

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
var graphClient = new GraphServiceClient(requestAdapter);

var requestBody = new Microsoft.Graph.Beta.Models.Security.SiteSource
{
	Site = new Site
	{
		WebUrl = "https://m365x809305.sharepoint.com/sites/Retail",
	},
};
var result = await graphClient.Security.Cases.EdiscoveryCases["ediscoveryCase-id"].Custodians["ediscoveryCustodian-id"].SiteSources.PostAsync(requestBody);


```