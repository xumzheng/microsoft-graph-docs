---
description: "Automatically generated file. DO NOT MODIFY"
---

```powershell

Import-Module Microsoft.Graph.Beta.WindowsUpdates

$params = @{
	addMembers = @(
		@{
			"@odata.type" = "#microsoft.graph.windowsUpdates.azureADDevice"
			id = "String (identifier)"
		}
	)
	removeMembers = @(
		@{
			"@odata.type" = "#microsoft.graph.windowsUpdates.azureADDevice"
			id = "String (identifier)"
		}
	)
	addExclusions = @(
		@{
			"@odata.type" = "#microsoft.graph.windowsUpdates.azureADDevice"
			id = "String (identifier)"
		}
	)
	removeExclusions = @(
		@{
			"@odata.type" = "#microsoft.graph.windowsUpdates.azureADDevice"
			id = "String (identifier)"
		}
	)
}

Update-MgBetaWindowsUpdatesDeploymentAudience -DeploymentId $deploymentId -BodyParameter $params

```