---
description: "Automatically generated file. DO NOT MODIFY"
---

```csharp

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
var graphClient = new GraphServiceClient(requestAdapter);

var requestBody = new User
{
	BusinessPhones = new List<>
	{
		"+1 425 555 0109",
	},
	OfficeLocation = "18/2111",
};
await graphClient.Users["user-id"].PatchAsync(requestBody);


```