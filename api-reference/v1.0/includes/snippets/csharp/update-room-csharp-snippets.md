---
description: "Automatically generated file. DO NOT MODIFY"
---

```csharp

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
var graphClient = new GraphServiceClient(requestAdapter);

var requestBody = new Place
{
	@odata.type = "microsoft.graph.room",
	AdditionalData = new()
	{
		{"nickname", "Conf Room"},
		{"building", "1"},
		{"label", "100"},
		{"capacity", },
		{"isWheelChairAccessible", false},
	}
};
await graphClient.Places["place-id"].PatchAsync(requestBody);


```