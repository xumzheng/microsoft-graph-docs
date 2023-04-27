---
description: "Automatically generated file. DO NOT MODIFY"
---

```powershellv2

Import-Module Microsoft.Graph.Beta.Applications

$params = @{
	criteria = @{
		resetScope = "Watermark, Escrows, QuarantineState"
	}
}

Restart-MgBetaServicePrincipalsSynchronizationJob -ServicePrincipalId $servicePrincipalId -SynchronizationJobId $synchronizationJobId -BodyParameter $params

```