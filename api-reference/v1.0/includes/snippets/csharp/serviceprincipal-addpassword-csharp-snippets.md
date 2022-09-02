---
description: "Automatically generated file. DO NOT MODIFY"
---

```csharp

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
var graphClient = new GraphServiceClient(requestAdapter);

var requestBody = new PasswordCredentialPostRequestBody
{
	PasswordCredential = new PasswordCredential
	{
		DisplayName = "Password friendly name",
	},
};
var result = await graphClient.ServicePrincipals["servicePrincipal-id"].AddPassword.PostAsync(requestBody);


```