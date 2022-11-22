---
description: "Automatically generated file. DO NOT MODIFY"
---

```powershellv2

Import-Module Microsoft.Graph.Beta.Users

$params = @{
	Name = "Leisure tasks"
}

# A UPN can also be used as -UserId.
New-MgBetaUserOutlookTaskGroup -UserId $userId -BodyParameter $params

```