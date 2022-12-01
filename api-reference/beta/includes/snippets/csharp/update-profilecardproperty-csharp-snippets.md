---
description: "Automatically generated file. DO NOT MODIFY"
---

```csharp

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
var graphClient = new GraphServiceClient(requestAdapter);

var requestBody = new ProfileCardProperty
{
	Annotations = new List<ProfileCardAnnotation>
	{
		new ProfileCardAnnotation
		{
			Localizations = new List<DisplayNameLocalization>
			{
				new DisplayNameLocalization
				{
					LanguageTag = "no-NB",
					DisplayName = "Kostnads Senter",
				},
			},
		},
	},
};
var result = await graphClient.Organization["organization-id"].Settings.ProfileCardProperties["profileCardProperty-id"].PatchAsync(requestBody);


```