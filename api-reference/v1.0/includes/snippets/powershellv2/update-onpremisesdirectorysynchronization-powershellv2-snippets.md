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
	}
	Features = @{
		GroupWriteBackEnabled = $true
	}
}

Update-MgBetaDirectoryOnPremiseSynchronization -OnPremisesDirectorySynchronizationId $onPremisesDirectorySynchronizationId -BodyParameter $params

```