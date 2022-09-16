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
			"displayName" , "Joni Sherman"
		},
		{
			"emailAddress" , "jonis@relecloud.com"
		},
		{
			"addresses" , new List<>
			{
				new 
				{
					PostOfficeBox = "",
					Street = "4567 Main Street",
					City = "Buffalo",
					State = "NY",
					CountryOrRegion = "USA",
					PostalCode = "98052",
					Type = "home",
				},
				new 
				{
					PostOfficeBox = "",
					Street = "4570 Main Street",
					City = "Buffalo",
					State = "NY",
					CountryOrRegion = "USA",
					PostalCode = "98054",
					Type = "business",
				},
			}
		},
		{
			"phones" , new List<>
			{
				new 
				{
					Number = "206-555-0100",
					Type = "home",
				},
				new 
				{
					Number = "206-555-0200",
					Type = "business",
				},
			}
		},
	},
};
var result = await graphClient.Solutions.BookingBusinesses["bookingBusiness-id"].Customers.PostAsync(requestBody);


```