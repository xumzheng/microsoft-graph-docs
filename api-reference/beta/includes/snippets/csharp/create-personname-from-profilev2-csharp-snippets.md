---
description: "Automatically generated file. DO NOT MODIFY"
---

```csharp

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
var graphClient = new GraphServiceClient(requestAdapter);

var requestBody = new PersonName
{
	DisplayName = "Innocenty Popov",
	First = "Innocenty",
	Initials = "IP",
	Last = "Popov",
	LanguageTag = "en-US",
	Maiden = null,
};
var result = await graphClient.Me.Profile.Names.PostAsync(requestBody);


```