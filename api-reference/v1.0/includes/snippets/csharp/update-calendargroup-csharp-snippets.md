---
description: "Automatically generated file. DO NOT MODIFY"
---

```csharp

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
var graphClient = new GraphServiceClient(requestAdapter);

var requestBody = new CalendarGroup
{
	Name = "name-value",
};
await graphClient.Me.CalendarGroups["calendarGroup-id"].PatchAsync(requestBody);


```