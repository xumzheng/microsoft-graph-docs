---
description: "Automatically generated file. DO NOT MODIFY"
---

```powershellv2

Import-Module Microsoft.Graph.Beta.Mail

$params = @{
	"@odata.type" = "#microsoft.graph.itemAttachment"
	Name = "Holiday event"
	Item = @{
		"@odata.type" = "microsoft.graph.event"
		Subject = "Discuss gifts for children"
	}
}

# A UPN can also be used as -UserId.
New-MgBetaUserMessageAttachment -UserId $userId -MessageId $messageId -BodyParameter $params

```