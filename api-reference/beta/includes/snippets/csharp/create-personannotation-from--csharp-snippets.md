---
description: "Automatically generated file. DO NOT MODIFY"
---

```csharp

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
var graphClient = new GraphServiceClient(requestAdapter);

var requestBody = new PersonAnnotation
{
	Detail = new ItemBody
	{
		ContentType = BodyType.Text,
		Content = "I am originally from Australia, but grew up in Moscow, Russia.",
	},
	DisplayName = "About Me",
};
var result = await graphClient.Me.Profile.Notes.PostAsync(requestBody);


```