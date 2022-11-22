---
description: "Automatically generated file. DO NOT MODIFY"
---

```powershellv1

Import-Module Microsoft.Graph.Security

$params = @{
	Classification = "TruePositive"
	Determination = "MultiStagedAttack"
	Tags = @(
		"Demo"
	)
}

Update-MgSecurityIncident -IncidentId $incidentId -BodyParameter $params

```