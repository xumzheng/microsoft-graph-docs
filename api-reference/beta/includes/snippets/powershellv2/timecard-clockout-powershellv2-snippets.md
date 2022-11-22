---
description: "Automatically generated file. DO NOT MODIFY"
---

```powershellv2

Import-Module Microsoft.Graph.Beta.Teams

$params = @{
	AtAprovedLocation = $true
	Notes = @{
		ContentType = "text"
		Content = "clock out smaple notes"
	}
}

Invoke-MgBetaClockTeamScheduleTimeCardOut -TeamId $teamId -TimeCardId $timeCardId -BodyParameter $params

```