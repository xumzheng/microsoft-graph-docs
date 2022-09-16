---
description: "Automatically generated file. DO NOT MODIFY"
---

```csharp

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
var graphClient = new GraphServiceClient(requestAdapter);

var requestBody = new UnifiedRoleAssignmentMultiple
{
	PrincipalIds = new List<string>
	{
		"0aeec2c1-fee7-4e02-b534-6f920d25b300",
		"2d5386a7-732f-44db-9cf8-f82dd2a1c0e0",
	},
};
await graphClient.RoleManagement.DeviceManagement.RoleAssignments["unifiedRoleAssignmentMultiple-id"].PatchAsync(requestBody);


```