---
description: "Automatically generated file. DO NOT MODIFY"
---

```csharp

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
var graphClient = new GraphServiceClient(requestAdapter);

var requestBody = new ServicePrincipal
{
	AppId = "65415bb1-9267-4313-bbf5-ae259732ee12",
};
var result = await graphClient.ServicePrincipals.PostAsync(requestBody);


```