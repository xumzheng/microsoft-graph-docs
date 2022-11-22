---
description: "Automatically generated file. DO NOT MODIFY"
---

```powershellv2

Import-Module Microsoft.Graph.Beta.Security

$params = @{
	Classification = "TruePositive"
	Determination = "MultiStagedAttack"
	Tags = @(
		"Demo"
	)
}

Update-MgBetaSecurityIncident -IncidentId $incidentId -BodyParameter $params

```