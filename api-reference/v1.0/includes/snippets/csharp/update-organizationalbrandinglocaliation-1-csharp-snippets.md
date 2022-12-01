---
description: "Automatically generated file. DO NOT MODIFY"
---

```csharp

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
var graphClient = new GraphServiceClient(requestAdapter);

var requestBody = new OrganizationalBranding
{
	SignInPageText = "Default",
	UsernameHintText = "DefaultHint",
};
var result = await graphClient.Organization["organization-id"].Branding.PatchAsync(requestBody, (requestConfiguration) =>
{
	requestConfiguration.Headers.Add("Accept-Language", "0");
});


```