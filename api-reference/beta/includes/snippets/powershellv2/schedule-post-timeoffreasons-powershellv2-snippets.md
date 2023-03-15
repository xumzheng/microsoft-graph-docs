---
description: "Automatically generated file. DO NOT MODIFY"
---

```powershellv2

Import-Module Microsoft.Graph.Beta.Teams

$params = @{
	DisplayName = "Vacation"
	IconType = "plane"
	IsActive = $true
}

New-MgBetaTeamScheduleTimeOffReason -TeamId $teamId -BodyParameter $params

```