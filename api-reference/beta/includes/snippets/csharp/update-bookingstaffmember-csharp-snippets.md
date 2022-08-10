---
description: "Automatically generated file. DO NOT MODIFY"
---

```csharp

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
var graphClient = new GraphServiceClient(requestAdapter);

var requestBody = new BookingStaffMember
{
	WorkingHours = new List<BookingWorkHours>
	{
		new BookingWorkHours
		{
			OdataType = "#microsoft.graph.bookingWorkHours",
			Day = DayOfWeek.Monday,
			TimeSlots = new List<>
			{
			},
			AdditionalData = new Dictionary<string, object>
			{
				{
					"day@odata.type" , "#microsoft.graph.dayOfWeek"
				},
				{
					"timeSlots@odata.type" , "#Collection(microsoft.graph.bookingWorkTimeSlot)"
				},
			},
		},
		new BookingWorkHours
		{
			OdataType = "#microsoft.graph.bookingWorkHours",
			Day = DayOfWeek.Tuesday,
			TimeSlots = new List<BookingWorkTimeSlot>
			{
				new BookingWorkTimeSlot
				{
					OdataType = "#microsoft.graph.bookingWorkTimeSlot",
					End = "17:00:00.0000000",
					Start = "08:00:00.0000000",
				},
			},
			AdditionalData = new Dictionary<string, object>
			{
				{
					"day@odata.type" , "#microsoft.graph.dayOfWeek"
				},
				{
					"timeSlots@odata.type" , "#Collection(microsoft.graph.bookingWorkTimeSlot)"
				},
			},
		},
		new BookingWorkHours
		{
			OdataType = "#microsoft.graph.bookingWorkHours",
			Day = DayOfWeek.Wednesday,
			TimeSlots = new List<BookingWorkTimeSlot>
			{
				new BookingWorkTimeSlot
				{
					OdataType = "#microsoft.graph.bookingWorkTimeSlot",
					End = "17:00:00.0000000",
					Start = "08:00:00.0000000",
				},
			},
			AdditionalData = new Dictionary<string, object>
			{
				{
					"day@odata.type" , "#microsoft.graph.dayOfWeek"
				},
				{
					"timeSlots@odata.type" , "#Collection(microsoft.graph.bookingWorkTimeSlot)"
				},
			},
		},
		new BookingWorkHours
		{
			OdataType = "#microsoft.graph.bookingWorkHours",
			Day = DayOfWeek.Thursday,
			TimeSlots = new List<BookingWorkTimeSlot>
			{
				new BookingWorkTimeSlot
				{
					OdataType = "#microsoft.graph.bookingWorkTimeSlot",
					End = "17:00:00.0000000",
					Start = "08:00:00.0000000",
				},
			},
			AdditionalData = new Dictionary<string, object>
			{
				{
					"day@odata.type" , "#microsoft.graph.dayOfWeek"
				},
				{
					"timeSlots@odata.type" , "#Collection(microsoft.graph.bookingWorkTimeSlot)"
				},
			},
		},
		new BookingWorkHours
		{
			OdataType = "#microsoft.graph.bookingWorkHours",
			Day = DayOfWeek.Friday,
			TimeSlots = new List<BookingWorkTimeSlot>
			{
				new BookingWorkTimeSlot
				{
					OdataType = "#microsoft.graph.bookingWorkTimeSlot",
					End = "17:00:00.0000000",
					Start = "08:00:00.0000000",
				},
			},
			AdditionalData = new Dictionary<string, object>
			{
				{
					"day@odata.type" , "#microsoft.graph.dayOfWeek"
				},
				{
					"timeSlots@odata.type" , "#Collection(microsoft.graph.bookingWorkTimeSlot)"
				},
			},
		},
	},
};
await graphClient.BookingBusinesses["bookingBusiness-id"].StaffMembers["bookingStaffMember-id"].PatchAsync(requestBody);


```