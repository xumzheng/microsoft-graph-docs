---
description: "Automatically generated file. DO NOT MODIFY"
---

```powershellv2

Import-Module Microsoft.Graph.Beta.Users.Actions

$params = @{
	AttachmentInfo = @{
		AttachmentType = "file"
		Name = "flower"
		Size = 3483322
	}
}

# A UPN can also be used as -UserId.
New-MgBetaUserTodoListTaskAttachmentUploadSession -UserId $userId -TodoTaskListId $todoTaskListId -TodoTaskId $todoTaskId -BodyParameter $params

```