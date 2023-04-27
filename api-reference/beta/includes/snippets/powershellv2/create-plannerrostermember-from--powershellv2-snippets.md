---
description: "Automatically generated file. DO NOT MODIFY"
---

```powershellv2

Import-Module Microsoft.Graph.Beta.Planner

$params = @{
	"@odata.type" = "#microsoft.graph.plannerRosterMember"
	userId = "String"
}

New-MgBetaPlannerRosterMember -PlannerRosterId $plannerRosterId -BodyParameter $params

```