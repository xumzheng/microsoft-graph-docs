---
description: "Automatically generated file. DO NOT MODIFY"
---

```powershell

Import-Module Microsoft.Graph.Teams

$params = @{
	"@microsoft.graph.teamCreationMode" = "migration"
	"Template@odata.bind" = "https://graph.microsoft.com/beta/teamsTemplates('standard')"
	DisplayName = "My Sample Team"
	Description = "My Sample Team’s Description"
	CreatedDateTime = [System.DateTime]::Parse("2020-03-14T11:22:17.067Z")
}

New-MgTeam -BodyParameter $params

```