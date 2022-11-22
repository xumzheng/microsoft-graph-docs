---
description: "Automatically generated file. DO NOT MODIFY"
---

```powershellv2

Import-Module Microsoft.Graph.Beta.Users.Actions

$params = @{
	CurrentPassword = "xWwvJ]6NMw+bWH-d"
	NewPassword = "0eM85N54wFxWwvJ]"
}

# A UPN can also be used as -UserId.
Update-MgBetaUserPassword -UserId $userId -BodyParameter $params

```