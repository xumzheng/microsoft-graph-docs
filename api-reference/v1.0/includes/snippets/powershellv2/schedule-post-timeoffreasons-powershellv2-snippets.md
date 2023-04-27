---
description: "Automatically generated file. DO NOT MODIFY"
---

```powershellv2

Import-Module Microsoft.Graph.Teams

$params = @{
	displayName = "Vacation"
	iconType = "plane"
	isActive = $true
}

New-MgTeamScheduleTimeOffReason -TeamId $teamId -BodyParameter $params

```