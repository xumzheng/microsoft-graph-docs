---
description: "Automatically generated file. DO NOT MODIFY"
---

```powershellv2

Import-Module Microsoft.Graph.Beta.Teams

$params = @{
	atAprovedLocation = $true
	notes = @{
		contentType = "text"
		content = "start break smaple notes"
	}
}

Start-MgBetaTeamScheduleTimeCardBreak -TeamId $teamId -TimeCardId $timeCardId -BodyParameter $params

```