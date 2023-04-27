---
description: "Automatically generated file. DO NOT MODIFY"
---

```powershellv2

Import-Module Microsoft.Graph.Beta.Teams

$params = @{
	"template@odata.bind" = "https://graph.microsoft.com/beta/teamsTemplates('educationClass')"
	displayName = "My Class Team"
	description = "My Class Team’s Description"
}

New-MgBetaTeam -BodyParameter $params

```