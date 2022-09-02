---
description: "Automatically generated file. DO NOT MODIFY"
---

```csharp

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
var graphClient = new GraphServiceClient(requestAdapter);

var requestBody = new GetPasswordSingleSignOnCredentialsPostRequestBody
{
	Id = "5793aa3b-cca9-4794-679a240f8b58",
};
var result = await graphClient.ServicePrincipals["servicePrincipal-id"].GetPasswordSingleSignOnCredentials.PostAsync(requestBody);


```