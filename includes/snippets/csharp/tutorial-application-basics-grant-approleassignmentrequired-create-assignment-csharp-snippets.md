---
description: "Automatically generated file. DO NOT MODIFY"
---

```csharp

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
var graphClient = new GraphServiceClient(requestAdapter);

var requestBody = new AppRoleAssignment
{
	PrincipalId = "b8afc02cb-4d62-4dba-b536-9f6d73e9e26",
	ResourceId = "89473e09-0737-41a1-a0c3-1418d6908bcd",
	AppRoleId = "00000000-0000-0000-0000-000000000000",
};
var result = await graphClient.ServicePrincipals["servicePrincipal-id"].AppRoleAssignedTo.PostAsync(requestBody);


```