---
description: "Automatically generated file. DO NOT MODIFY"
---

```powershellv1

Import-Module Microsoft.Graph.Applications

$params = @{
	PasswordCredential = @{
		DisplayName = "Password friendly name"
	}
}

Add-MgApplicationPassword -ApplicationId $applicationId -BodyParameter $params

```