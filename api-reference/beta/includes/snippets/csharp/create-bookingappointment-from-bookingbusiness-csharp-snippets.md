---
description: "Automatically generated file. DO NOT MODIFY"
---

```csharp

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
var graphClient = new GraphServiceClient(requestAdapter);

var requestBody = new BookingAppointment
{
	@odata.type = "#microsoft.graph.bookingAppointment",
	CustomerEmailAddress = "jordanm@contoso.com",
	CustomerLocation = new Location
	{
		@odata.type = "#microsoft.graph.location",
		Address = new PhysicalAddress
		{
			City = "Buffalo",
			CountryOrRegion = "USA",
			PostalCode = "98052",
			PostOfficeBox = null,
			State = "NY",
			Street = "123 First Avenue",
			Type = null,
			AdditionalData = new()
			{
				{"@odata.type", "#microsoft.graph.physicalAddress"},
				{"type@odata.type", "#microsoft.graph.physicalAddressType"},
			}
		},
		Coordinates = null,
		DisplayName = "Customer",
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
	CustomerName = "Jordan Miller",
	CustomerNotes = "Please be on time.",
	CustomerPhone = "213-555-0199",
	CustomerTimeZone = "America/Chicago",
	SmsNotificationsEnabled = true,
	End = new DateTimeTimeZone
	{
		DateTime = "2018-05-01T12:30:00.0000000+00:00",
		TimeZone = "UTC",
		AdditionalData = new()
		{
			{"@odata.type", "#microsoft.graph.dateTimeTimeZone"},
		}
	},
	InvoiceAmount = 10d,
	InvoiceDate = new DateTimeTimeZone
	{
		DateTime = "2018-05-01T12:30:00.0000000+00:00",
		TimeZone = "UTC",
		AdditionalData = new()
		{
			{"@odata.type", "#microsoft.graph.dateTimeTimeZone"},
		}
	},
	InvoiceId = "1001",
	InvoiceStatus = "open",
	InvoiceUrl = "theInvoiceUrl",
	IsLocationOnline = true,
	OptOutOfCustomerEmail = false,
	AnonymousJoinWebUrl = null,
	PostBuffer = "PT10M",
	PreBuffer = "PT5M",
	Price = 10d,
	PriceType = "fixedPrice",
	Reminders = new List<BookingReminder>
	{
		new BookingReminder
		{
			Message = "This service is tomorrow",
			Offset = "P1D",
			Recipients = "allAttendees",
			AdditionalData = new()
			{
				{"@odata.type", "#microsoft.graph.bookingReminder"},
				{"recipients@odata.type", "#microsoft.graph.bookingReminderRecipients"},
			}
		},
		new BookingReminder
		{
			Message = "Please be available to enjoy your lunch service.",
			Offset = "PT1H",
			Recipients = "customer",
			AdditionalData = new()
			{
				{"@odata.type", "#microsoft.graph.bookingReminder"},
				{"recipients@odata.type", "#microsoft.graph.bookingReminderRecipients"},
			}
		},
		new BookingReminder
		{
			Message = "Please check traffic for next cater.",
			Offset = "PT2H",
			Recipients = "staff",
			AdditionalData = new()
			{
				{"@odata.type", "#microsoft.graph.bookingReminder"},
				{"recipients@odata.type", "#microsoft.graph.bookingReminderRecipients"},
			}
		},
	}
	ServiceId = "57da6774-a087-4d69-b0e6-6fb82c339976",
	ServiceLocation = new Location
	{
		@odata.type = "#microsoft.graph.location",
		Address = new PhysicalAddress
		{
			City = "Buffalo",
			CountryOrRegion = "USA",
			PostalCode = "98052",
			PostOfficeBox = null,
			State = "NY",
			Street = "123 First Avenue",
			Type = null,
			AdditionalData = new()
			{
				{"@odata.type", "#microsoft.graph.physicalAddress"},
				{"type@odata.type", "#microsoft.graph.physicalAddressType"},
			}
		},
		Coordinates = null,
		DisplayName = "Customer location",
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
	ServiceName = "Catered bento",
	ServiceNotes = "Customer requires punctual service.",
	Start = new DateTimeTimeZone
	{
		DateTime = "2018-05-01T12:00:00.0000000+00:00",
		TimeZone = "UTC",
		AdditionalData = new()
		{
			{"@odata.type", "#microsoft.graph.dateTimeTimeZone"},
		}
	},
	MaximumAttendeesCount = 5,
	FilledAttendeesCount = 1,
	Customers = new List<BookingCustomerInformationBase>
	{
		new BookingCustomerInformationBase
		{
			AdditionalData = new()
			{
				{"@odata.type", "#microsoft.graph.bookingCustomerInformation"},
				{"customerId", "7ed53fa5-9ef2-4f2f-975b-27447440bc09"},
				{"name", "Jordan Miller"},
				{"emailAddress", "jordanm@contoso.com"},
				{"phone", "213-555-0199"},
				{"notes", null},
				{"timeZone", "America/Chicago"},
				{"customQuestionAnswers", new List<Object>
				{
				}
			}
		},
	}
	AdditionalData = new()
	{
		{"invoiceStatus@odata.type", "#microsoft.graph.bookingInvoiceStatus"},
		{"priceType@odata.type", "#microsoft.graph.bookingPriceType"},
		{"reminders@odata.type", "#Collection(microsoft.graph.bookingReminder)"},
	}
};
var result = await graphClient.BookingBusinesses["bookingBusiness-id"].Appointments.PostAsync(requestBody);


```