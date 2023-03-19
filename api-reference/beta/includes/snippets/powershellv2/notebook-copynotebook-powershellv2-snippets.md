---
description: "Automatically generated file. DO NOT MODIFY"
---

```powershellv2

Import-Module Microsoft.Graph.Beta.Users.Actions

$params = @{
	GroupId = "groupId-value"
	RenameAs = "renameAs-value"
}

# A UPN can also be used as -UserId.
Copy-MgBetaUserOnenoteNotebook -UserId $userId -NotebookId $notebookId -BodyParameter $params

```