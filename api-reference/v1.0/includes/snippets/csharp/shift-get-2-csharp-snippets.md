---
description: "Automatically generated file. DO NOT MODIFY"
---

```csharp

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
var graphClient = new GraphServiceClient(requestAdapter);

var requestBody = new ShiftPreferences
{
	Id = "SHPR_eeab4fb1-20e5-48ca-ad9b-98119d94bee7",
	Availability = new List<ShiftAvailability>
	{
		new ShiftAvailability
		{
			Recurrence = new PatternedRecurrence
			{
				Pattern = new RecurrencePattern
				{
					Type = RecurrencePatternType.Weekly,
					DaysOfWeek = new List<>
					{
						DayOfWeek.Monday,
						DayOfWeek.Wednesday,
						DayOfWeek.Friday,
					},
					Interval = 1,
				},
				Range = new RecurrenceRange
				{
					Type = RecurrenceRangeType.Noend,
				},
			},
			TimeZone = "Pacific Standard Time",
			TimeSlots = null,
		},
	},
	AdditionalData = new Dictionary<string, object>
	{
		{
			"@odata.etag" , "1a371e53-f0a6-4327-a1ee-e3c56e4b38aa"
		},
	},
};
await graphClient.Users["user-id"].Settings.ShiftPreferences.PatchAsync(requestBody);


```