---
description: "Automatically generated file. DO NOT MODIFY"
---

```powershellv2

Import-Module Microsoft.Graph.Bookings

$params = @{
	CancellationMessage = "Your appointment has been successfully cancelled. Please call us again."
}

Stop-MgsBookingBusinessesAppointment -BookingBusinessId $bookingBusinessId -BookingAppointmentId $bookingAppointmentId -BodyParameter $params

```