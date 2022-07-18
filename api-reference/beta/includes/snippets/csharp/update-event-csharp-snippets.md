---
description: "Automatically generated file. DO NOT MODIFY"
---

```csharp

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
var graphClient = new GraphServiceClient(requestAdapter);

var requestBody = new Event
{
	OriginalStartTimeZone = "originalStartTimeZone-value",
	OriginalEndTimeZone = "originalEndTimeZone-value",
	ResponseStatus = new ResponseStatus
	{
		Response = "",
		Time = DateTimeOffset.Parse("2016-10-19T10:37:00Z"),
	},
	Recurrence = null,
	Uid = "iCalUId-value",
	ReminderMinutesBeforeStart = 99,
	IsOnlineMeeting = true,
	OnlineMeetingProvider = "teamsForBusiness",
	IsReminderOn = true,
	HideAttendees = false,
	Categories = new List<String>
	{
		"Red category",
	}
};
await graphClient.Me.Events["event-id"].PatchAsync(requestBody);


```