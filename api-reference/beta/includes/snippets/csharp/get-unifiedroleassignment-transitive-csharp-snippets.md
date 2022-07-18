---
description: "Automatically generated file. DO NOT MODIFY"
---

```csharp

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
var graphClient = new GraphServiceClient(requestAdapter);

var result = await graphClient.RoleManagement.Directory.TransitiveRoleAssignments.GetAsync((requestConfiguration) =>
{
	requestConfiguration.QueryParameters.Count = true;
	requestConfiguration.QueryParameters.Filter = "principalId%20eq%20'2c7936bc-3517-40f3-8eda-4806637b6516'%20and%20roleDefinitionId%20eq%20'fe930be7-5e62-47db-91af-98c3a49a38b1'";
	requestConfiguration.Headers.Add("ConsistencyLevel", "eventual");
});


```