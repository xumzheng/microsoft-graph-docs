---
description: "Automatically generated file. DO NOT MODIFY"
---

```csharp

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
var graphClient = new GraphServiceClient(requestAdapter);

var requestBody = new BookingCustomerBase
{
	@odata.type = "#microsoft.graph.bookingCustomer",
	AdditionalData = new()
	{
		{"displayName", "Joni Sherman"},
		{"emailAddress", "jonis@relecloud.com"},
		{"addresses", new List<Object>
		{
		}
		{"phones", new List<Object>
		{
		}
	}
};
var result = await graphClient.Solutions.BookingBusinesses["bookingBusiness-id"].Customers.PostAsync(requestBody);


```