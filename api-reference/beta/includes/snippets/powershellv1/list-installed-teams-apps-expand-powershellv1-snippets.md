---
description: "Automatically generated file. DO NOT MODIFY"
---

```powershellv1

Import-Module Microsoft.Graph.Teams

Get-MgTeamInstalledApp -TeamId $teamId -ExpandProperty "teamsAppDefinition(`$expand=bot)" 

```