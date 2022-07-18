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
			Day = "monday",
			TimeSlots = new List<BookingWorkTimeSlot>
			{
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
};
await graphClient.BookingBusinesses["bookingBusiness-id"].StaffMembers["bookingStaffMember-id"].PatchAsync(requestBody);


```