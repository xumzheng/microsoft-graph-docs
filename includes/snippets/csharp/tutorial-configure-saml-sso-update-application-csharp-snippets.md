---
description: "Automatically generated file. DO NOT MODIFY"
---

```csharp

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
var graphClient = new GraphServiceClient(requestAdapter);

var requestBody = new Application
{
	Web = new WebApplication
	{
		RedirectUris = new List<string>
		{
			"https://signin.aws.amazon.com/saml",
		},
	},
	IdentifierUris = new List<string>
	{
		"https://signin.aws.amazon.com/saml",
	},
};
var result = await graphClient.Applications["application-id"].PatchAsync(requestBody);


```