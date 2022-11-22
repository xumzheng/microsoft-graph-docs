---
description: "Automatically generated file. DO NOT MODIFY"
---

```powershellv2

Import-Module Microsoft.Graph.Beta.Users

$params = @{
	Color = "preset15"
}

# A UPN can also be used as -UserId.
Update-MgBetaUserOutlookMasterCategory -UserId $userId -OutlookCategoryId $outlookCategoryId -BodyParameter $params

```