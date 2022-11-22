---
description: "Automatically generated file. DO NOT MODIFY"
---

```powershellv1

Import-Module Microsoft.Graph.Teams

$params = @{
	DisplayName = "Vacation"
	IconType = "plane"
	IsActive = $true
}

New-MgTeamScheduleTimeOffReason -TeamId $teamId -BodyParameter $params

```