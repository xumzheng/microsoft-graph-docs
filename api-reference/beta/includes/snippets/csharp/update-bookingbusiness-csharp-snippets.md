---
description: "Automatically generated file. DO NOT MODIFY"
---

```csharp

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
var graphClient = new GraphServiceClient(requestAdapter);

var requestBody = new BookingBusiness
{
	Email = "admin@fabrikam.com",
	SchedulingPolicy = new BookingSchedulingPolicy
	{
		TimeSlotInterval = "PT60M",
		MinimumLeadTime = "P1D",
		MaximumAdvance = "P30D",
		SendConfirmationsToOwner = true,
		AllowStaffSelection = true,
	},
};
await graphClient.BookingBusinesses["bookingBusiness-id"].PatchAsync(requestBody);


```