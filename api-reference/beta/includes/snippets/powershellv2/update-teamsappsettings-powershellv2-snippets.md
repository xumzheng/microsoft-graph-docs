---
description: "Automatically generated file. DO NOT MODIFY"
---

```powershellv2

Import-Module Microsoft.Graph.Beta.Teams

$params = @{
	"@odata.type" = "#microsoft.graph.teamsAppSettings"
	isChatResourceSpecificConsentEnabled = "true"
}

Update-MgBetaTeamworkTeamAppSetting -BodyParameter $params

```