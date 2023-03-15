---
description: "Automatically generated file. DO NOT MODIFY"
---

```powershellv2

Import-Module Microsoft.Graph.Teams

$params = @{
	DisplayName = "Finance"
}

Update-MgTeamTag -TeamId $teamId -TeamworkTagId $teamworkTagId -BodyParameter $params

```