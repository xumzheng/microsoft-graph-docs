---
description: "Automatically generated file. DO NOT MODIFY"
---

```csharp

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
var graphClient = new GraphServiceClient(requestAdapter);

var requestBody = new DelegatedAdminAccessAssignment
{
	AccessDetails = new DelegatedAdminAccessDetails
	{
		UnifiedRoles = new List<UnifiedRole>
		{
			new UnifiedRole
			{
				AdditionalData = new Dictionary<string, object>
				{
					{
						"roleDefinitionId" , "88d8e3e3-8f55-4a1e-953a-9b9898b8876b"
					},
				},
			},
			new UnifiedRole
			{
				AdditionalData = new Dictionary<string, object>
				{
					{
						"roleDefinitionId" , "44367163-eba1-44c3-98af-f5787879f96a"
					},
				},
			},
			new UnifiedRole
			{
				AdditionalData = new Dictionary<string, object>
				{
					{
						"roleDefinitionId" , "729827e3-9c14-49f7-bb1b-9608f156bbb8"
					},
				},
			},
		},
	},
};
await graphClient.TenantRelationships.DelegatedAdminRelationships["delegatedAdminRelationship-id"].AccessAssignments["delegatedAdminAccessAssignment-id"].PatchAsync(requestBody, (requestConfiguration) =>
{
	requestConfiguration.Headers.Add("If-Match", "W/\"JyI0NzAwNjg0NS0wMDAwLTE5MDAtMDAwMC02MGY0Yjg4MzAwMDAiJw==\"");
});


```