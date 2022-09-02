---
description: "Automatically generated file. DO NOT MODIFY"
---

```csharp

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
var graphClient = new GraphServiceClient(requestAdapter);

var requestBody = new CancelPostRequestBody
{
	CancellationMessage = "Your appointment has been successfully cancelled. Please call us again.",
};
await graphClient.BookingBusinesses["bookingBusiness-id"].Appointments["bookingAppointment-id"].Cancel.PostAsync(requestBody);


```