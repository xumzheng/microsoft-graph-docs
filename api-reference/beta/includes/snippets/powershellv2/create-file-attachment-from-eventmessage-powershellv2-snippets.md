---
description: "Automatically generated file. DO NOT MODIFY"
---

```powershellv2

Import-Module Microsoft.Graph.Beta.Mail

$params = @{
	"@odata.type" = "#Microsoft.OutlookServices.FileAttachment"
	Name = "name-value"
	ContentType = "contentType-value"
	IsInline = $false
	ContentLocation = "contentLocation-value"
	ContentBytes = "contentBytes-value"
}

# A UPN can also be used as -UserId.
New-MgBetaUserMessageAttachment -UserId $userId -MessageId $messageId -BodyParameter $params

```