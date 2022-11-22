---
description: "Automatically generated file. DO NOT MODIFY"
---

```powershellv2

Import-Module Microsoft.Graph.Beta.Teams

$params = @{
	"Template@odata.bind" = "https://graph.microsoft.com/beta/teamsTemplates('standard')"
	DisplayName = "My Sample Team"
	Description = "My Sample Team’s Description"
}

New-MgBetaTeam -BodyParameter $params

```