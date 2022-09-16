---
description: "Automatically generated file. DO NOT MODIFY"
---

```csharp

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
var graphClient = new GraphServiceClient(requestAdapter);

var requestBody = new ApprovalStage
{
	ReviewResult = "Approve",
	Justification = "OK",
};
await graphClient.IdentityGovernance.EntitlementManagement.AccessPackageAssignmentApprovals["approval-id"].Stages["approvalStage-id"].PatchAsync(requestBody);


```