---
description: "Automatically generated file. DO NOT MODIFY"
---

```csharp

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
var graphClient = new GraphServiceClient(requestAdapter);

var result = await graphClient.IdentityGovernance.EntitlementManagement.AccessPackageAssignmentRequests.GetAsync((requestConfiguration) =>
{
	requestConfiguration.QueryParameters.Expand = new [] { "requestor($expand=connectedOrganization)" };
	requestConfiguration.QueryParameters.Filter = "(requestState%20eq%20'PendingApproval')";
});


```