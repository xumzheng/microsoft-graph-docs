---
description: "Automatically generated file. DO NOT MODIFY"
---

```powershellv2

Import-Module Microsoft.Graph.Beta.Teams

$params = @{
	DisplayName = "Cashiers"
	IsActive = $true
	UserIds = @(
		"c5d0c76b-80c4-481c-be50-923cd8d680a1"
		"2a4296b3-a28a-44ba-bc66-0274b9b95851"
	)
}

New-MgBetaTeamScheduleSchedulingGroup -TeamId $teamId -BodyParameter $params

```