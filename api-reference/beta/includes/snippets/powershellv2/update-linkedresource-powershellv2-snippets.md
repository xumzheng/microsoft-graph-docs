---
description: "Automatically generated file. DO NOT MODIFY"
---

```powershellv2

Import-Module Microsoft.Graph.Beta.Users

$params = @{
	"@odata.type" = "#microsoft.graph.linkedResource"
	WebUrl = "http://microsoft.com"
	ApplicationName = "Microsoft"
	DisplayName = "Microsoft"
}

# A UPN can also be used as -UserId.
Update-MgBetaUserTodoListTaskLinkedResource -UserId $userId -TodoTaskListId $todoTaskListId -TodoTaskId $todoTaskId -LinkedResourceId $linkedResourceId -BodyParameter $params

```