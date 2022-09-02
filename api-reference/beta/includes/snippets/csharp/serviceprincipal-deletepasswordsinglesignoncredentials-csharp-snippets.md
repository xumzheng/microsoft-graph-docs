---
description: "Automatically generated file. DO NOT MODIFY"
---

```csharp

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
var graphClient = new GraphServiceClient(requestAdapter);

var requestBody = new DeletePasswordSingleSignOnCredentialsPostRequestBody
{
	Id = "5793aa3b-cca9-4794-679a240f8b58",
};
await graphClient.ServicePrincipals["servicePrincipal-id"].DeletePasswordSingleSignOnCredentials.PostAsync(requestBody);


```