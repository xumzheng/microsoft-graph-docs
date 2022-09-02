---
description: "Automatically generated file. DO NOT MODIFY"
---

```csharp

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
var graphClient = new GraphServiceClient(requestAdapter);

var requestBody = new AssociateWithHubSitesPostRequestBody
{
	HubSiteUrls = new List<>
	{
		"https://graph.microsoft.com/v1.0/sites/{site-id}",
	},
	PropagateToExistingLists = false,
};
await graphClient.Sites["site-id"].ContentTypes["contentType-id"].AssociateWithHubSites.PostAsync(requestBody);


```