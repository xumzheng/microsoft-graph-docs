---
description: "Automatically generated file. DO NOT MODIFY"
---

```csharp

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
var graphClient = new GraphServiceClient(requestAdapter);

var requestBody = new DirectoryRole
{
	RoleTemplateId = "fe930be7-5e62-47db-91af-98c3a49a38b1",
};
var result = await graphClient.DirectoryRoles.PostAsync(requestBody);


```