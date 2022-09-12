---
description: "Automatically generated file. DO NOT MODIFY"
---

```csharp

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
var graphClient = new GraphServiceClient(requestAdapter);

var requestBody = new PersonInterest
{
	Categories = new List<string>
	{
		"Sports",
	},
};
await graphClient.Me.Profile.Interests["personInterest-id"].PatchAsync(requestBody);


```