---
description: "Automatically generated file. DO NOT MODIFY"
---

```powershellv2

Import-Module Microsoft.Graph.Security

$params = @{
	Classification = "TruePositive"
	Determination = "MultiStagedAttack"
	CustomTags = @(
		"Demo"
	)
}

Update-MgSecurityIncident -IncidentId $incidentId -BodyParameter $params

```