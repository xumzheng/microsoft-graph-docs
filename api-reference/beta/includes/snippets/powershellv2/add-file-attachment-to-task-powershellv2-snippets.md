---
description: "Automatically generated file. DO NOT MODIFY"
---

```powershellv2

Import-Module Microsoft.Graph.Beta.Users

$params = @{
	"@odata.type" = "#microsoft.graph.fileAttachment"
	Name = "menu.txt"
	ContentBytes = "bWFjIGFuZCBjaGVlc2UgdG9kYXk="
}

# A UPN can also be used as -UserId.
New-MgBetaUserOutlookTaskAttachment -UserId $userId -OutlookTaskId $outlookTaskId -BodyParameter $params

```