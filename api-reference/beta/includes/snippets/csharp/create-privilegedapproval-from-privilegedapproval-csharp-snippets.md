---
description: "Automatically generated file. DO NOT MODIFY"
---

```csharp

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
var graphClient = new GraphServiceClient(requestAdapter);

var requestBody = new PrivilegedApproval
{
	UserId = "userId-value",
	RoleId = "roleId-value",
	ApprovalType = "approvalType-value",
	ApprovalState = ApprovalState.ApprovalState-value,
	ApprovalDuration = TimeSpan.Parse("datetime-value"),
};
var result = await graphClient.PrivilegedApproval.PostAsync(requestBody);


```