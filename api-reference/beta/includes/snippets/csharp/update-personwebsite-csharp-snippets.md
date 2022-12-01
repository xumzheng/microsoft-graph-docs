---
description: "Automatically generated file. DO NOT MODIFY"
---

```csharp

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
var graphClient = new GraphServiceClient(requestAdapter);

var requestBody = new PersonWebsite
{
	Description = "Lyn Damer play in the Women's 1st Division (Toppserien) in Norway",
};
var result = await graphClient.Me.Profile.Websites["personWebsite-id"].PatchAsync(requestBody);


```