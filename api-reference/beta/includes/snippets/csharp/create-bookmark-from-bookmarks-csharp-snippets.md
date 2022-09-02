---
description: "Automatically generated file. DO NOT MODIFY"
---

```csharp

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
var graphClient = new GraphServiceClient(requestAdapter);

var requestBody = new Microsoft.Graph.Beta..Search.Bookmark
{
	DisplayName = "Contoso Install Site",
	WebUrl = "http://www.contoso.com/",
	Description = "Try or buy Contoso for Home or Business and view product information",
	Keywords = new AnswerKeyword
	{
		Keywords = new List<string>
		{
			"Contoso",
			"install",
		},
		ReservedKeywords = new List<string>
		{
			"Contoso",
		},
		MatchSimilarKeywords = true,
	},
	AvailabilityStartDateTime = null,
	AvailabilityEndDateTime = null,
	Platforms = new List<>
	{
		DevicePlatformType.Windows,
	},
	TargetedVariations = new List<Microsoft.Graph.Beta..Search.AnswerVariant>
	{
		new AnswerVariant
		{
			LanguageTag = "es-es",
			DisplayName = "Sitio de instalación Contoso",
			Description = "Pruebe o compre Contoso hogar o negocios y vea la información del producto",
		},
	},
	State = AnswerState.Published,
};
var result = await graphClient.Search.Bookmarks.PostAsync(requestBody);


```