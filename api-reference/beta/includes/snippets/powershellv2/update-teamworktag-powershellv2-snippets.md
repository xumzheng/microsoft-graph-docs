---
description: "Automatically generated file. DO NOT MODIFY"
---

```powershellv2

Import-Module Microsoft.Graph.Beta.Teams

$params = @{
	DisplayName = "Finance"
}

Update-MgBetaTeamTag -TeamId $teamId -TeamworkTagId $teamworkTagId -BodyParameter $params

```