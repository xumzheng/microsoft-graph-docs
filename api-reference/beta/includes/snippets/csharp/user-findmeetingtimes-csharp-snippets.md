---
description: "Automatically generated file. DO NOT MODIFY"
---

```csharp

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
var graphClient = new GraphServiceClient(requestAdapter);

var requestBody = new FindMeetingTimesRequestBody
{
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
	LocationConstraint = new LocationConstraint
	{
		IsRequired = "false",
		SuggestLocation = "false",
		Locations = new List<Object>
		{
			new 
			{
				AdditionalData = new()
				{
					{"resolveAvailability", "false"},
					{"displayName", "Conf room Hood"},
				}
			},
		}
	},
	TimeConstraint = new TimeConstraint
	{
		ActivityDomain = "work",
		TimeSlots = new List<TimeSlot>
		{
			new TimeSlot
			{
				Start = new DateTimeTimeZone
				{
					DateTime = "2019-04-16T09:00:00",
					TimeZone = "Pacific Standard Time",
				},
				End = new DateTimeTimeZone
				{
					DateTime = "2019-04-18T17:00:00",
					TimeZone = "Pacific Standard Time",
				},
			},
		}
	},
	IsOrganizerOptional = "false",
	MeetingDuration = "PT1H",
	ReturnSuggestionReasons = "true",
	MinimumAttendeePercentage = "100",
};
var result = await graphClient.Me.FindMeetingTimes.PostAsync(requestBody, (requestConfiguration) =>
{
	requestConfiguration.Headers.Add("Prefer", "outlook.timezone="Pacific Standard Time"");
});


```