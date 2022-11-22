---
description: "Automatically generated file. DO NOT MODIFY"
---

```powershellv1

Import-Module Microsoft.Graph.Users

$params = @{
	Name = "Personal Tasks"
}

# A UPN can also be used as -UserId.
Update-MgUserOutlookTaskGroup -UserId $userId -OutlookTaskGroupId $outlookTaskGroupId -BodyParameter $params

```