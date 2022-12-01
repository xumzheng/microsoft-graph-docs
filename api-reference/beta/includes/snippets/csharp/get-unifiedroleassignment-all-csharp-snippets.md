---
description: "Automatically generated file. DO NOT MODIFY"
---

```csharp

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
var graphClient = new GraphServiceClient(requestAdapter);

var result = await graphClient.RoleManagement.DirectoryObject.TransitiveRoleAssignments.GetAsync((requestConfiguration) =>
{
	requestConfiguration.QueryParameters.Count = true;
	requestConfiguration.QueryParameters.Filter = "principalId eq '2c7936bc-3517-40f3-8eda-4806637b6516'";
	requestConfiguration.Headers.Add("ConsistencyLevel", "eventual");
});


```