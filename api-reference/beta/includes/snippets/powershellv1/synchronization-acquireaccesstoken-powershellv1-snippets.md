---
description: "Automatically generated file. DO NOT MODIFY"
---

```powershellv1

Import-Module Microsoft.Graph.Applications

$params = @{
	Credentials = @(
		@{
			"@odata.type" = "microsoft.graph.synchronizationSecretKeyStringValuePair"
		}
	)
}

Get-MgApplicationSynchronizationAccessToken -ApplicationId $applicationId -BodyParameter $params

```