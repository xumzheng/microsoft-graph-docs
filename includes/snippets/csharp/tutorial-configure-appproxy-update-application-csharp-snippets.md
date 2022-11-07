---
description: "Automatically generated file. DO NOT MODIFY"
---

```csharp

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
var graphClient = new GraphServiceClient(requestAdapter);

var requestBody = new Application
{
	IdentifierUris = new List<string>
	{
		"https://contosoiwaapp-contoso.msappproxy.net",
	},
	Web = new WebApplication
	{
		RedirectUris = new List<string>
		{
			"https://contosoiwaapp-contoso.msappproxy.net",
		},
		HomePageUrl = "https://contosoiwaapp-contoso.msappproxy.net",
	},
};
var result = await graphClient.Applications["application-id"].PatchAsync(requestBody);


```