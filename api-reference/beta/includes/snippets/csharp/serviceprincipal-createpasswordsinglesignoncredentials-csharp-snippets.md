---
description: "Automatically generated file. DO NOT MODIFY"
---

```csharp

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
var graphClient = new GraphServiceClient(requestAdapter);

var requestBody = new CreatePasswordSingleSignOnCredentialsPostRequestBody
{
	Id = "5793aa3b-cca9-4794-679a240f8b58",
	Credentials = new List<Credential>
	{
		new Credential
		{
			AdditionalData = new Dictionary<string, object>
			{
				{
					"fieldId" , "param_username"
				},
				{
					"value" , "myusername"
				},
				{
					"type" , "username"
				},
			},
		},
		new Credential
		{
			AdditionalData = new Dictionary<string, object>
			{
				{
					"fieldId" , "param_password"
				},
				{
					"value" , "pa$$w0rd"
				},
				{
					"type" , "password"
				},
			},
		},
	},
};
var result = await graphClient.ServicePrincipals["servicePrincipal-id"].CreatePasswordSingleSignOnCredentials.PostAsync(requestBody);


```