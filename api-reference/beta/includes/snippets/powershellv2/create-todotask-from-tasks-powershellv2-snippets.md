---
description: "Automatically generated file. DO NOT MODIFY"
---

```powershellv2

Import-Module Microsoft.Graph.Beta.Users

$params = @{
	Title = "A new task"
	Categories = @(
		"Important"
	)
	LinkedResources = @(
		@{
			WebUrl = "http://microsoft.com"
			ApplicationName = "Microsoft"
			DisplayName = "Microsoft"
		}
	)
}

# A UPN can also be used as -UserId.
New-MgBetaUserTodoListTask -UserId $userId -TodoTaskListId $todoTaskListId -BodyParameter $params

```