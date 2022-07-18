---
description: "Automatically generated file. DO NOT MODIFY"
---

```csharp

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
var graphClient = new GraphServiceClient(requestAdapter);

var result = await graphClient.Solutions.BookingBusinesses["bookingBusiness-id"].CalendarView.GetAsync((requestConfiguration) =>
{
	requestConfiguration.QueryParameters.Start = "2018-04-30T00:00:00Z";
	requestConfiguration.QueryParameters.End = "2018-05-10T00:00:00Z";
});


```