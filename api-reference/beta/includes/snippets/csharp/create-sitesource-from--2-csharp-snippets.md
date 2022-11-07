---
description: "Automatically generated file. DO NOT MODIFY"
---

```csharp

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
var graphClient = new GraphServiceClient(requestAdapter);

var requestBody = new Microsoft.Graph.Beta.Models.Ediscovery.SiteSource
{
	Site = new Site
	{
		WebUrl = "https://contoso.sharepoint.com/sites/SecretSite",
	},
};
var result = await graphClient.Compliance.Ediscovery.Cases["case-id"].LegalHolds["legalHold-id"].SiteSources.PostAsync(requestBody);


```