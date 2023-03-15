---
description: "Automatically generated file. DO NOT MODIFY"
---

```powershellv2

Import-Module Microsoft.Graph.Beta.Teams

$params = @{
	DisplayName = "Architecture Discussion"
	Description = "This channel is where we debate all future architecture plans"
	MembershipType = "standard"
}

New-MgBetaTeamChannel -TeamId $teamId -BodyParameter $params

```