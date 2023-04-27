---
description: "Automatically generated file. DO NOT MODIFY"
---

```powershellv2

Import-Module Microsoft.Graph.Bookings

$params = @{
	"@odata.type" = "#microsoft.graph.bookingCustomQuestion"
	displayName = "What is your age?"
	answerInputType = "text"
	answerOptions = @(
	)
}

New-MgBookingBusinessCustomQuestion -BookingBusinessId $bookingBusinessId -BodyParameter $params

```