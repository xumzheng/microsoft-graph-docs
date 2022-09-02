---
description: "Automatically generated file. DO NOT MODIFY"
---

```csharp

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
var graphClient = new GraphServiceClient(requestAdapter);

var requestBody = new AccessPackageAssignmentPolicie
{
	AdditionalData = new Dictionary<string, object>
	{
		{
			"id" , "4540a08f-8ab5-43f6-a923-015275799197"
		},
		{
			"displayName" , "policy with custom access package workflow extension"
		},
		{
			"description" , "Run specified custom access package workflow extension at different stages."
		},
		{
			"accessPackageId" , "ba5807c7-2aa9-4c8a-907e-4a17ee587500"
		},
		{
			"expiration" , new 
			{
				Type = "afterDuration",
				Duration = "P365D",
			}
		},
		{
			"requestApprovalSettings" , null
		},
		{
			"requestorSettings" , new 
			{
				AcceptRequests = true,
				ScopeType = "AllExistingDirectorySubjects",
				AllowedRequestors = new List<>
				{
				},
			}
		},
		{
			"accessReviewSettings" , null
		},
		{
			"customExtensionHandlers" , new List<>
			{
			}
		},
	},
};
await graphClient.IdentityGovernance.EntitlementManagement.AccessPackageAssignmentPolicies["accessPackageAssignmentPolicy-id"].PutAsync(requestBody);


```