---
description: "Automatically generated file. DO NOT MODIFY"
---

```csharp

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
var graphClient = new GraphServiceClient(requestAdapter);

var requestBody = new Microsoft.Graph.Beta.Organization.Item.Branding.BrandingDeleteRequestBody
{
	AdditionalData = new Dictionary<string, object>
	{
		{
			"id" , "0"
		},
	},
};
await graphClient.Organization["organization-id"].Branding.DeleteAsync(requestBody);


```