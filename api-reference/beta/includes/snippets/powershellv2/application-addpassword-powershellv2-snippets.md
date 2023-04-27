---
description: "Automatically generated file. DO NOT MODIFY"
---

```powershellv2

Import-Module Microsoft.Graph.Beta.Applications

$params = @{
	passwordCredential = @{
		displayName = "Password friendly name"
	}
}

Add-MgBetaApplicationPassword -ApplicationId $applicationId -BodyParameter $params

```