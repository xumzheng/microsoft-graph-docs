---
description: "Automatically generated file. DO NOT MODIFY"
---

```powershell

Import-Module Microsoft.Graph.Teams

$params = @{
	atAprovedLocation = $true
	notes = @{
		contentType = "text"
		content = "end break smaple notes"
	}
}

Stop-MgTeamScheduleTimeCardBreak -TeamId $teamId -TimeCardId $timeCardId -BodyParameter $params

```