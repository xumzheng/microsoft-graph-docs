---
description: "Automatically generated file. DO NOT MODIFY"
---

```powershellv2

Import-Module Microsoft.Graph.Beta.Devices.CloudPrint

$params = @{
	status = @{
		state = "completed"
		description = "completed"
	}
}

Update-MgBetaPrintTaskDefinitionTask -PrintTaskDefinitionId $printTaskDefinitionId -PrintTaskId $printTaskId -BodyParameter $params

```