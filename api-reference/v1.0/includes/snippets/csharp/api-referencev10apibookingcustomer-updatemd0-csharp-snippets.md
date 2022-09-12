---
description: "Automatically generated file. DO NOT MODIFY"
---

```csharp

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
var graphClient = new GraphServiceClient(requestAdapter);

var requestBody = new BookingCustomerBase
{
	OdataType = "#microsoft.graph.bookingCustomer",
	AdditionalData = new Dictionary<string, object>
	{
		{
			"displayName" , "Adele"
		},
		{
			"emailAddress" , "adele@relecloud.com"
		},
	},
};
await graphClient.Solutions.BookingBusinesses["bookingBusiness-id"].Customers["bookingCustomerBase-id"].PatchAsync(requestBody);


```