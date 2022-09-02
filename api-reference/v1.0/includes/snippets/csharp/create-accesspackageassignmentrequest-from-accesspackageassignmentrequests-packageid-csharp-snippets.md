---
description: "Automatically generated file. DO NOT MODIFY"
---

```csharp

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
var graphClient = new GraphServiceClient(requestAdapter);

var requestBody = new AccessPackageAssignmentRequest
{
	RequestType = AccessPackageRequestType.UserAdd,
	Assignment = new Assignment
	{
		AdditionalData = new Dictionary<string, object>
		{
			{
				"accessPackageId" , "d7be3253-b9c6-4fab-adef-30d30de8da2b"
			},
		},
	},
};
var result = await graphClient.IdentityGovernance.EntitlementManagement.AssignmentRequests.PostAsync(requestBody);


```