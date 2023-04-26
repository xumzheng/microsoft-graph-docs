---
description: "Automatically generated file. DO NOT MODIFY"
---

```powershell

Import-Module Microsoft.Graph.Beta.Teams

$params = @{
	enabled = $true
	timeZone = "America/Chicago"
	provisionStatus = "Completed"
	provisionStatusCode = $null
	openShiftsEnabled = $true
	swapShiftsRequestsEnabled = $true
	offerShiftRequestsEnabled = $true
	timeOffRequestsEnabled = $true
	timeClockEnabled = $true
	timeClockSettings = @{
		approvedLocation = @{
			altitude = 1024.13
			latitude = 26.13246
			longitude = 24.34616
		}
	}
}

Set-MgBetaTeamSchedule -TeamId $teamId -BodyParameter $params

```