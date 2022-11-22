---
description: "Automatically generated file. DO NOT MODIFY"
---

```powershellv2

Import-Module Microsoft.Graph.Beta.Teams

$params = @{
	NotifyTeam = $true
	StartDateTime = [System.DateTime]::Parse("2018-10-08T00:00:00.000Z")
	EndDateTime = [System.DateTime]::Parse("2018-10-15T00:00:00.000Z")
}

Invoke-MgBetaShareTeamSchedule -TeamId $teamId -BodyParameter $params

```