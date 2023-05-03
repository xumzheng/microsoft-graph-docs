---
description: "Automatically generated file. DO NOT MODIFY"
---

```csharp

// Code snippets are only available for the latest version. Current version is 5.x

var graphClient = new GraphServiceClient(requestAdapter);

var requestBody = new PrivilegedApproval
{
	ApprovalState = ApprovalState.Pending,
	ApproverReason = "approverReason-value",
};
var result = await graphClient.PrivilegedApproval["{privilegedApproval-id}"].PatchAsync(requestBody);


```