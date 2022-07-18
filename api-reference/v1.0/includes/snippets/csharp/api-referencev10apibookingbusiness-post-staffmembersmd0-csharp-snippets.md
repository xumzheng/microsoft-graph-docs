---
description: "Automatically generated file. DO NOT MODIFY"
---

```csharp

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
var graphClient = new GraphServiceClient(requestAdapter);

var requestBody = new BookingStaffMemberBase
{
	@odata.type = "#microsoft.graph.bookingStaffMember",
	AdditionalData = new()
	{
		{"displayName", "Dana Swope"},
		{"emailAddress", "danas@contoso.com"},
		{"role@odata.type", "#microsoft.graph.bookingStaffRole"},
		{"role", "externalGuest"},
		{"timeZone", "America/Chicago"},
		{"useBusinessHours", true},
		{"workingHours@odata.type", "#Collection(microsoft.graph.bookingWorkHours)"},
		{"workingHours", new List<Object>
		{
		}
	}
};
var result = await graphClient.Solutions.BookingBusinesses["bookingBusiness-id"].StaffMembers.PostAsync(requestBody);


```