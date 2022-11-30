---
description: "Automatically generated file. DO NOT MODIFY"
---

```powershellv2

Import-Module Microsoft.Graph.Beta.Teams

$params = @{
	"@microsoft.graph.channelCreationMode" = "migration"
	DisplayName = "Import_150958_99z"
	Description = "Import_150958_99z"
	CreatedDateTime = [System.DateTime]::Parse("2020-03-14T11:22:17.067Z")
}

New-MgBetaTeamChannel -TeamId $teamId -BodyParameter $params

```