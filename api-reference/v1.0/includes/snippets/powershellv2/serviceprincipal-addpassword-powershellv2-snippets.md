---
description: "Automatically generated file. DO NOT MODIFY"
---

```powershellv2

Import-Module Microsoft.Graph.Applications

$params = @{
	PasswordCredential = @{
		DisplayName = "Password friendly name"
	}
}

Add-MgServicePrincipalPassword -ServicePrincipalId $servicePrincipalId -BodyParameter $params

```