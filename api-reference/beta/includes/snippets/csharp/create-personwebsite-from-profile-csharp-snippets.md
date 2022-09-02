---
description: "Automatically generated file. DO NOT MODIFY"
---

```csharp

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
var graphClient = new GraphServiceClient(requestAdapter);

var requestBody = new PersonWebsite
{
	Categories = new List<>
	{
		"football",
	},
	DisplayName = "Lyn Damer",
	WebUrl = "www.lyndamer.no",
};
var result = await graphClient.Me.Profile.Websites.PostAsync(requestBody);


```