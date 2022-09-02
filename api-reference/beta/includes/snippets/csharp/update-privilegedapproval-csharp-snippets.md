---
description: "Automatically generated file. DO NOT MODIFY"
---

```csharp

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
var graphClient = new GraphServiceClient(requestAdapter);

var requestBody = new PrivilegedApproval
{
	ApprovalState = ApprovalState.Pending,
	ApproverReason = "approverReason-value",
};
await graphClient.PrivilegedApproval["privilegedApproval-id"].PatchAsync(requestBody);


```