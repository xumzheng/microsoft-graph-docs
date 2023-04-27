---
description: "Automatically generated file. DO NOT MODIFY"
---

```powershellv2

Import-Module Microsoft.Graph.Beta.Users

$params = @{
	passwordProfile = @{
		forceChangePasswordNextSignIn = $true
		password = "xWwvJ]6NMw+bWH-d"
	}
}

Update-MgBetaUser -UserId $userId -BodyParameter $params

```