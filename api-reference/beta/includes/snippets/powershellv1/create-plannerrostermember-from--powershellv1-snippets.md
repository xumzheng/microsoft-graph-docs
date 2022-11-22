---
description: "Automatically generated file. DO NOT MODIFY"
---

```powershellv1

Import-Module Microsoft.Graph.Planner

$params = @{
	"@odata.type" = "#microsoft.graph.plannerRosterMember"
	UserId = "String"
}

New-MgPlannerRosterMember -PlannerRosterId $plannerRosterId -BodyParameter $params

```