---
description: "Automatically generated file. DO NOT MODIFY"
---

```powershellv2

Import-Module Microsoft.Graph.Beta.Users

$params = @{
	DueDateTime = @{
		DateTime = "2020-07-25T16:00:00"
		TimeZone = "Eastern Standard Time"
	}
}

# A UPN can also be used as -UserId.
Update-MgBetaUserTodoListTask -UserId $userId -TodoTaskListId $todoTaskListId -TodoTaskId $todoTaskId -BodyParameter $params

```