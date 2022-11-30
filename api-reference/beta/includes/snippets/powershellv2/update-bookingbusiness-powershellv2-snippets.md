---
description: "Automatically generated file. DO NOT MODIFY"
---

```powershellv2

Import-Module Microsoft.Graph.Beta.Bookings

$params = @{
	Email = "admin@fabrikam.com"
	SchedulingPolicy = @{
		TimeSlotInterval = "PT60M"
		MinimumLeadTime = "P1D"
		MaximumAdvance = "P30D"
		SendConfirmationsToOwner = $true
		AllowStaffSelection = $true
	}
}

Update-MgBetaBookingBusiness -BookingBusinessId $bookingBusinessId -BodyParameter $params

```