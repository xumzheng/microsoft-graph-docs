---
description: "Automatically generated file. DO NOT MODIFY"
---

```csharp

// Code snippets are only available for the latest version. Current version is 5.x

var graphClient = new GraphServiceClient(requestAdapter);

var requestBody = new PrivilegedRoleAssignment
{
	UserId = "userId-value",
	RoleId = "roleId-value",
};
var result = await graphClient.PrivilegedRoleAssignments.PostAsync(requestBody);


```