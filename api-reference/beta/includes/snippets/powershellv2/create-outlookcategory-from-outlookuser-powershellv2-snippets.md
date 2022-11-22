---
description: "Automatically generated file. DO NOT MODIFY"
---

```powershellv2

Import-Module Microsoft.Graph.Beta.Users

$params = @{
	DisplayName = "Project expenses"
	Color = "preset9"
}

# A UPN can also be used as -UserId.
New-MgBetaUserOutlookMasterCategory -UserId $userId -BodyParameter $params

```