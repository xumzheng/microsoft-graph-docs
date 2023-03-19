---
description: "Automatically generated file. DO NOT MODIFY"
---

```powershellv2

Import-Module Microsoft.Graph.Beta.Identity.DirectoryManagement

$params = @{
	Configuration = @{
		AccidentalDeletionPrevention = @{
			SynchronizationPreventionType = "enabledForCount"
			AlertThreshold = 500
		}
		SynchronizationInterval = "PT30M"
		CustomerRequestedSynchronizationInterval = "PT1H"
	}
	Features = @{
		GroupWriteBackEnabled = $true
	}
}

Update-MgBetaDirectoryOnPremiseSynchronization -OnPremisesDirectorySynchronizationId $onPremisesDirectorySynchronizationId -BodyParameter $params

```