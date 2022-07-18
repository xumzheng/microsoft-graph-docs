---
description: "Automatically generated file. DO NOT MODIFY"
---

```csharp

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
var graphClient = new GraphServiceClient(requestAdapter);

var requestBody = new BookingStaffMember
{
	@odata.type = "#microsoft.graph.bookingStaffMember",
	ColorIndex = 1,
	DisplayName = "Dana Swope",
	EmailAddress = "danas@contoso.com",
	Role = "externalGuest",
	TimeZone = "America/Chicago",
	UseBusinessHours = true,
	WorkingHours = new List<BookingWorkHours>
	{
		new BookingWorkHours
		{
			Day = "monday",
			TimeSlots = new List<BookingWorkTimeSlot>
			{
				new BookingWorkTimeSlot
				{
					End = "17:00:00.0000000",
					Start = "08:00:00.0000000",
					AdditionalData = new()
					{
						{"@odata.type", "#microsoft.graph.bookingWorkTimeSlot"},
					}
				},
			}
			AdditionalData = new()
			{
				{"@odata.type", "#microsoft.graph.bookingWorkHours"},
				{"day@odata.type", "#microsoft.graph.dayOfWeek"},
				{"timeSlots@odata.type", "#Collection(microsoft.graph.bookingWorkTimeSlot)"},
			}
		},
		new BookingWorkHours
		{
			Day = "tuesday",
			TimeSlots = new List<BookingWorkTimeSlot>
			{
				new BookingWorkTimeSlot
				{
					End = "17:00:00.0000000",
					Start = "08:00:00.0000000",
					AdditionalData = new()
					{
						{"@odata.type", "#microsoft.graph.bookingWorkTimeSlot"},
					}
				},
			}
			AdditionalData = new()
			{
				{"@odata.type", "#microsoft.graph.bookingWorkHours"},
				{"day@odata.type", "#microsoft.graph.dayOfWeek"},
				{"timeSlots@odata.type", "#Collection(microsoft.graph.bookingWorkTimeSlot)"},
			}
		},
		new BookingWorkHours
		{
			Day = "wednesday",
			TimeSlots = new List<BookingWorkTimeSlot>
			{
				new BookingWorkTimeSlot
				{
					End = "17:00:00.0000000",
					Start = "08:00:00.0000000",
					AdditionalData = new()
					{
						{"@odata.type", "#microsoft.graph.bookingWorkTimeSlot"},
					}
				},
			}
			AdditionalData = new()
			{
				{"@odata.type", "#microsoft.graph.bookingWorkHours"},
				{"day@odata.type", "#microsoft.graph.dayOfWeek"},
				{"timeSlots@odata.type", "#Collection(microsoft.graph.bookingWorkTimeSlot)"},
			}
		},
		new BookingWorkHours
		{
			Day = "thursday",
			TimeSlots = new List<BookingWorkTimeSlot>
			{
				new BookingWorkTimeSlot
				{
					End = "17:00:00.0000000",
					Start = "08:00:00.0000000",
					AdditionalData = new()
					{
						{"@odata.type", "#microsoft.graph.bookingWorkTimeSlot"},
					}
				},
			}
			AdditionalData = new()
			{
				{"@odata.type", "#microsoft.graph.bookingWorkHours"},
				{"day@odata.type", "#microsoft.graph.dayOfWeek"},
				{"timeSlots@odata.type", "#Collection(microsoft.graph.bookingWorkTimeSlot)"},
			}
		},
		new BookingWorkHours
		{
			Day = "friday",
			TimeSlots = new List<BookingWorkTimeSlot>
			{
				new BookingWorkTimeSlot
				{
					End = "17:00:00.0000000",
					Start = "08:00:00.0000000",
					AdditionalData = new()
					{
						{"@odata.type", "#microsoft.graph.bookingWorkTimeSlot"},
					}
				},
			}
			AdditionalData = new()
			{
				{"@odata.type", "#microsoft.graph.bookingWorkHours"},
				{"day@odata.type", "#microsoft.graph.dayOfWeek"},
				{"timeSlots@odata.type", "#Collection(microsoft.graph.bookingWorkTimeSlot)"},
			}
		},
	}
	IsEmailNotificationEnabled = false,
	AdditionalData = new()
	{
		{"role@odata.type", "#microsoft.graph.bookingStaffRole"},
		{"workingHours@odata.type", "#Collection(microsoft.graph.bookingWorkHours)"},
	}
};
var result = await graphClient.BookingBusinesses["bookingBusiness-id"].StaffMembers.PostAsync(requestBody);


```