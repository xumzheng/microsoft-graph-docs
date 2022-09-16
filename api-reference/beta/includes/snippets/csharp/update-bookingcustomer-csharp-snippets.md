---
description: "Automatically generated file. DO NOT MODIFY"
---

```csharp

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
var graphClient = new GraphServiceClient(requestAdapter);

var requestBody = new BookingCustomer
{
	DisplayName = "Adele",
	EmailAddress = "adele@relecloud.com",
};
await graphClient.BookingBusinesses["bookingBusiness-id"].Customers["bookingCustomer-id"].PatchAsync(requestBody);


```