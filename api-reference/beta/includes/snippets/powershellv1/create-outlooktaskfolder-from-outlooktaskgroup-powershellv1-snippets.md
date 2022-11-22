---
description: "Automatically generated file. DO NOT MODIFY"
---

```powershellv1

Import-Module Microsoft.Graph.Users

$params = @{
	Name = "Cooking"
}

# A UPN can also be used as -UserId.
New-MgUserOutlookTaskGroupTaskFolder -UserId $userId -OutlookTaskGroupId $outlookTaskGroupId -BodyParameter $params

```