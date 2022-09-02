---
description: "Automatically generated file. DO NOT MODIFY"
---

```csharp

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
var graphClient = new GraphServiceClient(requestAdapter);

var requestBody = new ApplyPostRequestBody
{
	TenantId = "String",
	TenantGroupId = "String",
	ManagementTemplateId = "String",
};
var result = await graphClient.TenantRelationships.ManagedTenants.ManagementActions["managementAction-id"].Apply.PostAsync(requestBody);


```