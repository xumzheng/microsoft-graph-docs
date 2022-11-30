---
description: "Automatically generated file. DO NOT MODIFY"
---

```powershellv2

Import-Module Microsoft.Graph.Beta.Teams

$params = @{
	Enabled = $true
	TimeZone = "America/Chicago"
}

Set-MgBetaTeamSchedule -TeamId $teamId -BodyParameter $params

```