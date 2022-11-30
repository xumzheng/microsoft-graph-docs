---
description: "Automatically generated file. DO NOT MODIFY"
---

```powershellv2

Import-Module Microsoft.Graph.Beta.Teams

$params = @{
	"Template@odata.bind" = "https://graph.microsoft.com/beta/teamsTemplates('educationClass')"
	DisplayName = "My Class Team"
	Description = "My Class Team’s Description"
}

New-MgBetaTeam -BodyParameter $params

```