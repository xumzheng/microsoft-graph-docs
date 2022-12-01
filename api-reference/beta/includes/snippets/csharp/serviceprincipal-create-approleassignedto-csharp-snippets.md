---
description: "Automatically generated file. DO NOT MODIFY"
---

```csharp

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
var graphClient = new GraphServiceClient(requestAdapter);

var requestBody = new AppRoleAssignment
{
	PrincipalId = "33ad69f9-da99-4bed-acd0-3f24235cb296",
	ResourceId = "9028d19c-26a9-4809-8e3f-20ff73e2d75e",
	AppRoleId = "ef7437e6-4f94-4a0a-a110-a439eb2aa8f7",
};
var result = await graphClient.ServicePrincipals["servicePrincipal-id"].AppRoleAssignedTo.PostAsync(requestBody);


```