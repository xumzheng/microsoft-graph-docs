---
description: "Automatically generated file. DO NOT MODIFY"
---

```powershellv2

Import-Module Microsoft.Graph.Beta.Notes

$params = @{
	DisplayName = "My Private notebook"
}

# A UPN can also be used as -UserId.
New-MgBetaUserOnenoteNotebook -UserId $userId -BodyParameter $params

```