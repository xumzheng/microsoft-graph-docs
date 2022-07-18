---
description: "Automatically generated file. DO NOT MODIFY"
---

```csharp

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
var graphClient = new GraphServiceClient(requestAdapter);

var requestBody = new BookingService
{
	@odata.type = "#microsoft.graph.bookingService",
	DefaultDuration = "PT1H30M",
	DefaultLocation = new Location
	{
		@odata.type = "#microsoft.graph.location",
		Address = new PhysicalAddress
		{
			City = "Buffalo",
			CountryOrRegion = "USA",
			PostalCode = "98052",
			State = "NY",
			Street = "4567 First Street",
			AdditionalData = new()
			{
				{"@odata.type", "#microsoft.graph.physicalAddress"},
				{"postOfficeBox", null},
				{"type@odata.type", "#microsoft.graph.physicalAddressType"},
				{"type", null},
			}
		},
		Coordinates = null,
		DisplayName = "Contoso Lunch Delivery",
		LocationEmailAddress = null,
		LocationType = null,
		LocationUri = null,
		UniqueId = null,
		UniqueIdType = null,
		AdditionalData = new()
		{
			{"locationType@odata.type", "#microsoft.graph.locationType"},
			{"uniqueIdType@odata.type", "#microsoft.graph.locationUniqueIdType"},
		}
	},
	DefaultPrice = 10d,
	DefaultPriceType = "fixedPrice",
	DefaultReminders = new List<BookingReminder>
	{
		new BookingReminder
		{
			Message = "Please be reminded that this service is tomorrow.",
			Offset = "P1D",
			Recipients = "allAttendees",
			AdditionalData = new()
			{
				{"@odata.type", "#microsoft.graph.bookingReminder"},
				{"recipients@odata.type", "#microsoft.graph.bookingReminderRecipients"},
			}
		},
	}
	Description = "Individual bento box lunch delivery",
	DisplayName = "Bento",
	IsLocationOnline = true,
	SmsNotificationsEnabled = true,
	IsHiddenFromCustomers = false,
	Notes = "Home-cooked special",
	PostBuffer = "PT10M",
	PreBuffer = "PT5M",
	SchedulingPolicy = new BookingSchedulingPolicy
	{
		AllowStaffSelection = true,
		MaximumAdvance = "P10D",
		MinimumLeadTime = "PT10H",
		SendConfirmationsToOwner = true,
		TimeSlotInterval = "PT1H",
		AdditionalData = new()
		{
			{"@odata.type", "#microsoft.graph.bookingSchedulingPolicy"},
		}
	},
	StaffMemberIds = new List<String>
	{
		"d90d1e8c-5cfe-48cf-a2d5-966267375b6a",
		"2f5f8794-0b29-45b5-b56a-2eb5ff7aa880",
	}
	AdditionalData = new()
	{
		{"defaultPriceType@odata.type", "#microsoft.graph.bookingPriceType"},
		{"defaultReminders@odata.type", "#Collection(microsoft.graph.bookingReminder)"},
		{"staffMemberIds@odata.type", "#Collection(String)"},
	}
};
var result = await graphClient.Solutions.BookingBusinesses["bookingBusiness-id"].Services.PostAsync(requestBody);


```