---
description: "Automatically generated file. DO NOT MODIFY"
---

```powershellv2

Import-Module Microsoft.Graph.Applications

$params = @{
	passwordCredential = @{
		displayName = "Password friendly name"
	}
}

Add-MgApplicationPassword -ApplicationId $applicationId -BodyParameter $params

```