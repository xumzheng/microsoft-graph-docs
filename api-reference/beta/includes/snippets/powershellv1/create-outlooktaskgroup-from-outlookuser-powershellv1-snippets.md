---
description: "Automatically generated file. DO NOT MODIFY"
---

```powershellv1

Import-Module Microsoft.Graph.Users

$params = @{
	Name = "Leisure tasks"
}

# A UPN can also be used as -UserId.
New-MgUserOutlookTaskGroup -UserId $userId -BodyParameter $params

```