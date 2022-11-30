---
description: "Automatically generated file. DO NOT MODIFY"
---

```powershellv2

Import-Module Microsoft.Graph.Beta.Teams

$params = @{
	SenderMessage = "Can I take this shift?"
	OpenShiftId = "577b75d2-a927-48c0-a5d1-dc984894e7b8"
}

New-MgBetaTeamScheduleOpenShiftChangeRequest -TeamId $teamId -BodyParameter $params

```