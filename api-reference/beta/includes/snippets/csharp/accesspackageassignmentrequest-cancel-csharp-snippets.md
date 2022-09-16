---
description: "Automatically generated file. DO NOT MODIFY"
---

```csharp

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
var graphClient = new GraphServiceClient(requestAdapter);

var requestBody = new Microsoft.Graph.Beta.IdentityGovernance.EntitlementManagement.AccessPackageAssignmentRequests.Item.Cancel.CancelPostRequestBody
{
	AdditionalData = new Dictionary<string, object>
	{
		{
			"id" , "request-id"
		},
		{
			"requestStatus" , "cancelled"
		},
	},
};
await graphClient.IdentityGovernance.EntitlementManagement.AccessPackageAssignmentRequests["accessPackageAssignmentRequest-id"].Cancel.PostAsync(requestBody);


```