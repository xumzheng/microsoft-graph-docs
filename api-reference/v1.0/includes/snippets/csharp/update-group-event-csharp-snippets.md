---
description: "Automatically generated file. DO NOT MODIFY"
---

```csharp

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
var graphClient = new GraphServiceClient(requestAdapter);

var requestBody = new Event
{
	Location = new Location
	{
		DisplayName = "Conf Room 2",
	},
};
var result = await graphClient.Groups["group-id"].Calendar.Events["event-id"].PatchAsync(requestBody);


```