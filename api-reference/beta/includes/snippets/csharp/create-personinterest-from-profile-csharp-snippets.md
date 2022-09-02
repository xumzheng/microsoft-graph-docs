---
description: "Automatically generated file. DO NOT MODIFY"
---

```csharp

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
var graphClient = new GraphServiceClient(requestAdapter);

var requestBody = new PersonInterest
{
	Categories = new List<>
	{
		"Sports",
	},
	Description = "World's greatest football club",
	DisplayName = "Chelsea FC",
	WebUrl = "https://www.chelseafc.com",
};
var result = await graphClient.Me.Profile.Interests.PostAsync(requestBody);


```