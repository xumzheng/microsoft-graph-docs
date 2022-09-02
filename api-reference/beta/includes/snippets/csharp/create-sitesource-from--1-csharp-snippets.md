---
description: "Automatically generated file. DO NOT MODIFY"
---

```csharp

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
var graphClient = new GraphServiceClient(requestAdapter);

var requestBody = new Microsoft.Graph.Beta..Ediscovery.SiteSource
{
	Site = new Site
	{
		WebUrl = "https://contoso.sharepoint.com/sites/HumanResources",
	},
};
var result = await graphClient.Compliance.Ediscovery.Cases["case-id"].Custodians["custodian-id"].SiteSources.PostAsync(requestBody);


```