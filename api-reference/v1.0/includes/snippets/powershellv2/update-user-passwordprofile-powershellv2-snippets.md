---
description: "Automatically generated file. DO NOT MODIFY"
---

```powershellv2

Import-Module Microsoft.Graph.Users

$params = @{
	passwordProfile = @{
		forceChangePasswordNextSignIn = $false
		password = "xWwvJ]6NMw+bWH-d"
	}
}

Update-MgUser -UserId $userId -BodyParameter $params

```