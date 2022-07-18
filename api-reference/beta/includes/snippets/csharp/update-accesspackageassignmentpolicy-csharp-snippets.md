---
description: "Automatically generated file. DO NOT MODIFY"
---

```csharp

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
var graphClient = new GraphServiceClient(requestAdapter);

var requestBody = new AccessPackageAssignmentPolicy-idRequestBody
{
	AdditionalData = new()
	{
		{"id", "b2eba9a1-b357-42ee-83a8-336522ed6cbf"},
		{"accessPackageId", "4c02f928-7752-49aa-8fc8-e286d973a965"},
		{"displayName", "All Users"},
		{"description", "All users can request for access to the directory."},
		{"canExtend", false},
		{"durationInDays", },
		{"expirationDateTime", null},
		{"questions", new List<Object>
		{
		}
	}
};
await graphClient.IdentityGovernance.EntitlementManagement.AccessPackageAssignmentPolicies["accessPackageAssignmentPolicy-id"].PutAsync(requestBody);


```