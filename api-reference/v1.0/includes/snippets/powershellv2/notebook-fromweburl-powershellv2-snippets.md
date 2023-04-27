---
description: "Automatically generated file. DO NOT MODIFY"
---

```powershellv2

Import-Module Microsoft.Graph.Users.Actions

$params = @{
	webUrl = "webUrl value"
}

# A UPN can also be used as -UserId.
Get-MgUserOnenoteNotebookFromWebUrl -UserId $userId -BodyParameter $params

```