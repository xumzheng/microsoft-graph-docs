---
description: "Automatically generated file. DO NOT MODIFY"
---

```powershellv2

Import-Module Microsoft.Graph.Beta.Applications

$params = @{
	"@odata.id" = "https://graph.microsoft.com/onPremisesPublishingProfiles/applicationproxy/connectorGroups/{id}"
}

Set-MgBetaApplicationConnectorGroupByRef -ApplicationId $applicationId -BodyParameter $params

```