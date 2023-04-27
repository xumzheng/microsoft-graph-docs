---
description: "Automatically generated file. DO NOT MODIFY"
---

```powershellv2

Import-Module Microsoft.Graph.Security

$params = @{
	classification = "TruePositive"
	determination = "MultiStagedAttack"
	customTags = @(
		"Demo"
	)
}

Update-MgSecurityIncident -IncidentId $incidentId -BodyParameter $params

```