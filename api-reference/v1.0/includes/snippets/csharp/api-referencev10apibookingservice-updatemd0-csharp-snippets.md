---
description: "Automatically generated file. DO NOT MODIFY"
---

```csharp

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
var graphClient = new GraphServiceClient(requestAdapter);

var requestBody = new BookingService
{
	OdataType = "#microsoft.graph.bookingService",
	DefaultDuration = TimeSpan.Parse("PT30M"),
};
var result = await graphClient.Solutions.BookingBusinesses["bookingBusiness-id"].Services["bookingService-id"].PatchAsync(requestBody);


```