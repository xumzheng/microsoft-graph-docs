---
description: "Automatically generated file. DO NOT MODIFY"
---

```csharp

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
var graphClient = new GraphServiceClient(requestAdapter);

var requestBody = new Microsoft.Graph.ServicePrincipals.Item.Owners.Item.Ref.$refDeleteRequestBody
{
	AdditionalData = new Dictionary<string, object>
	{
		{
			"@odata.id" , "https://graph.microsoft.com/v1.0/directoryObjects/{id}"
		},
	},
};
await graphClient.ServicePrincipals["servicePrincipal-id"].Owners["directoryObject-id"].Ref.DeleteAsync(requestBody);


```