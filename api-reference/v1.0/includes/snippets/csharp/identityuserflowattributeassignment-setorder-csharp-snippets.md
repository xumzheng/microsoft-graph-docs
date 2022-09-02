---
description: "Automatically generated file. DO NOT MODIFY"
---

```csharp

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
var graphClient = new GraphServiceClient(requestAdapter);

var requestBody = new Microsoft.Graph.Beta.Identity.B2xUserFlows.Item.UserAttributeAssignments.SetOrder.SetOrderPostRequestBody
{
	NewAssignmentOrder = new AssignmentOrder
	{
		Order = new List<string>
		{
			"City",
			"extension_GUID_ShoeSize",
		},
	},
};
await graphClient.Identity.B2xUserFlows["b2xIdentityUserFlow-id"].UserAttributeAssignments.SetOrder.PostAsync(requestBody);


```