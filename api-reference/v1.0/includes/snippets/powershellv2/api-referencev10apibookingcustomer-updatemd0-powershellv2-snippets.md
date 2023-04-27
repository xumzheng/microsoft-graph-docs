---
description: "Automatically generated file. DO NOT MODIFY"
---

```powershellv2

Import-Module Microsoft.Graph.Bookings

$params = @{
	"@odata.type" = "#microsoft.graph.bookingCustomer"
	displayName = "Adele"
	emailAddress = "adele@relecloud.com"
}

Update-MgBookingBusinessCustomer -BookingBusinessId $bookingBusinessId -BookingCustomerBaseId $bookingCustomerBaseId -BodyParameter $params

```