---
description: "Automatically generated file. DO NOT MODIFY"
---

```csharp

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
var graphClient = new GraphServiceClient(requestAdapter);

var requestBody = new AccessPackageAssignmentPolicy
{
	AccessPackageId = "56ff43fd-6b05-48df-9634-956a777fce6d",
	DisplayName = "direct",
	Description = "direct assignments by administrator",
	AccessReviewSettings = null,
	RequestorSettings = new RequestorSettings
	{
		ScopeType = "NoSubjects",
		AcceptRequests = true,
		AllowedRequestors = new List<>
		{
		},
	},
	RequestApprovalSettings = new ApprovalSettings
	{
		IsApprovalRequired = false,
		IsApprovalRequiredForExtension = false,
		IsRequestorJustificationRequired = false,
		ApprovalMode = "NoApproval",
		ApprovalStages = new List<>
		{
		},
	},
};
var result = await graphClient.IdentityGovernance.EntitlementManagement.AccessPackageAssignmentPolicies.PostAsync(requestBody);


```