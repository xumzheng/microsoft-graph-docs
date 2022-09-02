---
description: "Automatically generated file. DO NOT MODIFY"
---

```csharp

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
var graphClient = new GraphServiceClient(requestAdapter);

var requestBody = new AccessPackageAssignmentRequest
{
	RequestType = "AdminAdd",
	AccessPackageAssignment = new AccessPackageAssignment
	{
		Target = new Target
		{
			Email = "user@contoso.com",
		},
		AssignmentPolicyId = "2264bf65-76ba-417b-a27d-54d291f0cbc8",
		AccessPackageId = "a914b616-e04e-476b-aa37-91038f0b165b",
	},
};
var result = await graphClient.IdentityGovernance.EntitlementManagement.AccessPackageAssignmentRequests.PostAsync(requestBody);


```