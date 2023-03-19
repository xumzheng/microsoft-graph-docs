---
description: "Automatically generated file. DO NOT MODIFY"
---

```powershellv2

Import-Module Microsoft.Graph.Beta.WindowsUpdates

$params = @{
	"@odata.type" = "#microsoft.graph.windowsUpdates.deployment"
	State = @{
		"@odata.type" = "microsoft.graph.windowsUpdates.deploymentState"
		RequestedValue = "paused"
	}
}

Update-MgBetaWindowsUpdatesDeployment -DeploymentId $deploymentId -BodyParameter $params

```