---
description: "Automatically generated file. DO NOT MODIFY"
---

```powershellv1

Import-Module Microsoft.Graph.Teams

$params = @{
	"@odata.type" = "#microsoft.graph.teamsAppSettings"
	IsChatResourceSpecificConsentEnabled = "true"
}

Update-MgTeamworkTeamAppSetting -BodyParameter $params

```