---
description: "Automatically generated file. DO NOT MODIFY"
---

```csharp

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
var graphClient = new GraphServiceClient(requestAdapter);

var requestBody = new BookingAppointment
{
	@odata.type = "#microsoft.graph.bookingAppointment",
	EndDateTime = new DateTimeTimeZone
	{
		DateTime = "2018-05-06T12:30:00.0000000+00:00",
		TimeZone = "UTC",
		AdditionalData = new()
		{
			{"@odata.type", "#microsoft.graph.dateTimeTimeZone"},
		}
	},
	StartDateTime = new DateTimeTimeZone
	{
		DateTime = "2018-05-06T12:00:00.0000000+00:00",
		TimeZone = "UTC",
		AdditionalData = new()
		{
			{"@odata.type", "#microsoft.graph.dateTimeTimeZone"},
		}
	},
};
await graphClient.Solutions.BookingBusinesses["bookingBusiness-id"].Appointments["bookingAppointment-id"].PatchAsync(requestBody);


```