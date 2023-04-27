---
description: "Automatically generated file. DO NOT MODIFY"
---

```powershellv2

Import-Module Microsoft.Graph.Devices.CloudPrint

$params = @{
	status = @{
		state = "completed"
		description = "completed"
	}
}

Update-MgPrintTaskDefinitionTask -PrintTaskDefinitionId $printTaskDefinitionId -PrintTaskId $printTaskId -BodyParameter $params

```