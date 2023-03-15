---
description: "Automatically generated file. DO NOT MODIFY"
---

```powershellv2

Import-Module Microsoft.Graph.Beta.Notes

$params = @{
	DisplayName = "Section group name"
}

# A UPN can also be used as -UserId.
New-MgBetaUserOnenoteNotebookSectionGroup -UserId $userId -NotebookId $notebookId -BodyParameter $params

```