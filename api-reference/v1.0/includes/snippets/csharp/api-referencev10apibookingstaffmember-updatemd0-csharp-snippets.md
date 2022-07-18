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
		{"workingHours", new List<Object>
		{
		}
	}
};
await graphClient.Solutions.BookingBusinesses["bookingBusiness-id"].StaffMembers["bookingStaffMemberBase-id"].PatchAsync(requestBody);


```