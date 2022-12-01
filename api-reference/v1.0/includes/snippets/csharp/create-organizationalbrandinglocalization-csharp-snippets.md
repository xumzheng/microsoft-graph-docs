---
description: "Automatically generated file. DO NOT MODIFY"
---

```csharp

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
var graphClient = new GraphServiceClient(requestAdapter);

var requestBody = new OrganizationalBrandingLocalization
{
	BackgroundColor = "#00000F",
	Id = "fr-FR",
	SignInPageText = " ",
};
var result = await graphClient.Organization["organization-id"].Branding.Localizations.PostAsync(requestBody);


```