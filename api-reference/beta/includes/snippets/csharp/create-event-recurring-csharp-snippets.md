---
description: "Automatically generated file. DO NOT MODIFY"
---

```csharp

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
var graphClient = new GraphServiceClient(requestAdapter);

var requestBody = new Event
{
	Subject = "Let's go for lunch",
	Body = new ItemBody
	{
		ContentType = "HTML",
		Content = "Does noon time work for you?",
	},
	Start = new DateTimeTimeZone
	{
		DateTime = "2017-09-04T12:00:00",
		TimeZone = "Pacific Standard Time",
	},
	End = new DateTimeTimeZone
	{
		DateTime = "2017-09-04T14:00:00",
		TimeZone = "Pacific Standard Time",
	},
	Recurrence = new PatternedRecurrence
	{
		Pattern = new RecurrencePattern
		{
			Type = "weekly",
			Interval = 1,
			DaysOfWeek = new List<DayOfWeek>
			{
				"Monday",
			}
		},
		Range = new RecurrenceRange
		{
			Type = "endDate",
			StartDate = "2017-09-04",
			EndDate = "2017-12-31",
		},
	},
	Location = new Location
	{
		DisplayName = "Harry's Bar",
	},
	Attendees = new List<Object>
	{
		new 
		{
			AdditionalData = new()
			{
				{"type", "required"},
			}
		},
	}
};
var result = await graphClient.Me.Events.PostAsync(requestBody);


```