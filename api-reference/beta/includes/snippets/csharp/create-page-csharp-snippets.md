---
description: "Automatically generated file. DO NOT MODIFY"
---

```csharp

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
var graphClient = new GraphServiceClient(requestAdapter);

var requestBody = new SitePage
{
	Name = "Events.aspx",
	Title = "Team Events",
	PublishingState = new PublicationFacet
	{
		Level = "checkedOut",
		VersionId = "0.1",
	},
	WebParts = new List<WebPart>
	{
		new WebPart
		{
			Type = "rte",
			Data = new SitePageData
			{
				AdditionalData = new()
				{
					{"innerHTML", "<p>Here are the team's upcoming events:</p>"},
				}
			},
		},
		new WebPart
		{
			Type = "d1d91016-032f-456d-98a4-721247c305e8",
			Data = new SitePageData
			{
				AdditionalData = new()
				{
					{"title", "Events"},
					{"description", "Display upcoming events"},
					{"dataVersion", "1.0"},
				}
			},
		},
	}
};
var result = await graphClient.Sites["site-id"].Pages.PostAsync(requestBody);


```