---
description: "Automatically generated file. DO NOT MODIFY"
---

```powershellv2

Import-Module Microsoft.Graph.Beta.Users

$params = @{
	DisplayName = "Vacation Plan"
}

# A UPN can also be used as -UserId.
Update-MgBetaUserTodoList -UserId $userId -TodoTaskListId $todoTaskListId -BodyParameter $params

```