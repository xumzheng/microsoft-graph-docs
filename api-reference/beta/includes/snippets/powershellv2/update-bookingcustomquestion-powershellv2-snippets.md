---
description: "Automatically generated file. DO NOT MODIFY"
---

```powershellv2

Import-Module Microsoft.Graph.Beta.Bookings

$params = @{
	"@odata.type" = "#microsoft.graph.bookingCustomQuestion"
	DisplayName = "What is your age?"
	AnswerInputType = "text"
	AnswerOptions = @(
	)
}

Update-MgBetaBookingBusinessCustomQuestion -BookingBusinessId $bookingBusinessId -BookingCustomQuestionId $bookingCustomQuestionId -BodyParameter $params

```