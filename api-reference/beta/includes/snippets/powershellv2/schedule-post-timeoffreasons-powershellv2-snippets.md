---
description: "Automatically generated file. DO NOT MODIFY"
---

```powershellv2

Import-Module Microsoft.Graph.Beta.Teams

$params = @{
	displayName = "Vacation"
	iconType = "plane"
	isActive = $true
}

New-MgBetaTeamScheduleTimeOffReason -TeamId $teamId -BodyParameter $params

```