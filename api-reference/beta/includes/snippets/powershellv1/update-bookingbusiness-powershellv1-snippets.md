---
description: "Automatically generated file. DO NOT MODIFY"
---

```powershellv1

Import-Module Microsoft.Graph.Bookings

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

Update-MgBookingBusiness -BookingBusinessId $bookingBusinessId -BodyParameter $params

```