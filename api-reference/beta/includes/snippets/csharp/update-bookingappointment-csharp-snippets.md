---
description: "Automatically generated file. DO NOT MODIFY"
---

```csharp

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
var graphClient = new GraphServiceClient(requestAdapter);

var requestBody = new BookingAppointment
{
	OdataType = "#microsoft.graph.bookingAppointment",
	End = new DateTimeTimeZone
	{
		OdataType = "#microsoft.graph.dateTimeTimeZone",
		DateTime = "2018-05-06T12:30:00.0000000+00:00",
		TimeZone = "UTC",
	},
	InvoiceDate = new DateTimeTimeZone
	{
		OdataType = "#microsoft.graph.dateTimeTimeZone",
		DateTime = "2018-05-06T12:30:00.0000000+00:00",
		TimeZone = "UTC",
	},
	Start = new DateTimeTimeZone
	{
		OdataType = "#microsoft.graph.dateTimeTimeZone",
		DateTime = "2018-05-06T12:00:00.0000000+00:00",
		TimeZone = "UTC",
	},
};
await graphClient.BookingBusinesses["bookingBusiness-id"].Appointments["bookingAppointment-id"].PatchAsync(requestBody);


```