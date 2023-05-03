---
description: "Automatically generated file. DO NOT MODIFY"
---

```csharp

// Code snippets are only available for the latest version. Current version is 5.x

var graphClient = new GraphServiceClient(requestAdapter);

var requestBody = new Microsoft.Graph.Beta.Applications.Item.AppManagementPolicies.Ref.$refDeleteRequestBody
{
	AdditionalData = new Dictionary<string, object>
	{
		{
			"@odata.id" , "https://graph.microsoft.com/beta/policies/appManagementPolicies/{id}"
		},
	},
};
await graphClient.Applications["{application-id}"].AppManagementPolicies.Ref.DeleteAsync(requestBody);


```