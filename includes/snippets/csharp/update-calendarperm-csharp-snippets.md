---
description: "Automatically generated file. DO NOT MODIFY"
---

```csharp

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
var graphClient = new GraphServiceClient(requestAdapter);

var requestBody = new CalendarPermission
{
	Role = CalendarRoleType.Write,
};
var result = await graphClient.Users["user-id"].Calendars["calendar-id"].CalendarPermissions["calendarPermission-id"].PatchAsync(requestBody);


```