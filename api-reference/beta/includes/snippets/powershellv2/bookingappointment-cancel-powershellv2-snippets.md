---
description: "Automatically generated file. DO NOT MODIFY"
---

```powershellv2

Import-Module Microsoft.Graph.Beta.Bookings

$params = @{
	cancellationMessage = "Your appointment has been successfully cancelled. Please call us again."
}

Stop-MgBetaBookingBusinessesAppointment -BookingBusinessId $bookingBusinessId -BookingAppointmentId $bookingAppointmentId -BodyParameter $params

```