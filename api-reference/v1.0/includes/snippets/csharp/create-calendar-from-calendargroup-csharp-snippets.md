---
description: "Automatically generated file. DO NOT MODIFY"
---

```csharp

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
var graphClient = new GraphServiceClient(requestAdapter);

var requestBody = new Calendar
{
	Name = "Marketing calendar",
};
var result = await graphClient.Me.CalendarGroups["calendarGroup-id"].Calendars.PostAsync(requestBody);


```