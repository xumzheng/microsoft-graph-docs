---
description: "Automatically generated file. DO NOT MODIFY"
---

```powershellv2

Import-Module Microsoft.Graph.Beta.Bookings

$params = @{
	"@odata.type" = "#microsoft.graph.businessScenarioTask"
	Title = "Customer order #12010"
	PercentComplete = 20
	Priority = 1
	BusinessScenarioProperties = @{
		ExternalObjectVersion = "000003"
	}
}

Update-MgBetaBusinessScenarioPlannerTask -BusinessScenarioId $businessScenarioId -BusinessScenarioTaskId $businessScenarioTaskId -BodyParameter $params

```