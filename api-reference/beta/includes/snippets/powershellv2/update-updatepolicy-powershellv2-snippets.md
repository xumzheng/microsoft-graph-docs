---
description: "Automatically generated file. DO NOT MODIFY"
---

```powershellv2

Import-Module Microsoft.Graph.Beta.WindowsUpdates

$params = @{
	"@odata.type" = "#microsoft.graph.windowsUpdates.updatePolicy"
	DeploymentSettings = @{
		"@odata.type" = "microsoft.graph.windowsUpdates.deploymentSettings"
		Schedule = @{
			GradualRollout = @{
				"@odata.type" = "#microsoft.graph.windowsUpdates.rateDrivenRolloutSettings"
				DurationBetweenOffers = "P1D"
				DevicePerOffer = 
			}
		}
	}
}

Update-MgBetaWindowsUpdatesPolicy -UpdatePolicyId $updatePolicyId -BodyParameter $params

```