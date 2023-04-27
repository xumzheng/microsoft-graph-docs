---
description: "Automatically generated file. DO NOT MODIFY"
---

```powershellv2

Import-Module Microsoft.Graph.Beta.WindowsUpdates

$params = @{
	"@odata.type" = "#microsoft.graph.windowsUpdates.deployment"
	state = @{
		"@odata.type" = "microsoft.graph.windowsUpdates.deploymentState"
		requestedValue = "paused"
	}
}

Update-MgBetaWindowsUpdatesDeployment -DeploymentId $deploymentId -BodyParameter $params

```