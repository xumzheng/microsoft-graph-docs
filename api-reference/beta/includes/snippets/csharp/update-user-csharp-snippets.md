---
description: "Automatically generated file. DO NOT MODIFY"
---

> [!NOTE]
> Code snippets are only available for the latest version. Current version is 5.x

```csharp

var graphClient = new GraphServiceClient(requestAdapter);

var requestBody = new User
{
	BusinessPhones = new List<string>
	{
		"+1 425 555 0109",
	},
	OfficeLocation = "18/2111",
};
var result = await graphClient.Me.PatchAsync(requestBody);


```
