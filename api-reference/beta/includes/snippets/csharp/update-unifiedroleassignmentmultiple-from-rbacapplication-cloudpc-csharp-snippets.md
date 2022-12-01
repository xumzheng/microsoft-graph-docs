---
description: "Automatically generated file. DO NOT MODIFY"
---

```csharp

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
var graphClient = new GraphServiceClient(requestAdapter);

var requestBody = new UnifiedRoleAssignmentMultiple
{
	DisplayName = "NewName",
	Description = "A new roleAssignment",
};
var result = await graphClient.RoleManagement.CloudPC.RoleAssignments["unifiedRoleAssignmentMultiple-id"].PatchAsync(requestBody);


```