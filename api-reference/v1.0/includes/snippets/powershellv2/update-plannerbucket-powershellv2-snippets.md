---
description: "Automatically generated file. DO NOT MODIFY"
---

```powershellv2

Import-Module Microsoft.Graph.Planner

$params = @{
	Name = "Development"
}

Update-MgPlannerBucket -PlannerBucketId $plannerBucketId -BodyParameter $params

```