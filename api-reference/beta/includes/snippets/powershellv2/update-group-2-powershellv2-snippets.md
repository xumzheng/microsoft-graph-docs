---
description: "Automatically generated file. DO NOT MODIFY"
---

```powershellv2

Import-Module Microsoft.Graph.Beta.Groups

$params = @{
	AssignedLabels = @(
		@{
			LabelId = "45cd0c48-c540-4358-ad79-a3658cdc5b88"
		}
	)
}

Update-MgBetaGroup -GroupId $groupId -BodyParameter $params

```