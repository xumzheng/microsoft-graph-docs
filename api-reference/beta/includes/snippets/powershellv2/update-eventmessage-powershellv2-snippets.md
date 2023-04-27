---
description: "Automatically generated file. DO NOT MODIFY"
---

```powershellv2

Import-Module Microsoft.Graph.Beta.Mail

$params = @{
	isRead = "true"
}

# A UPN can also be used as -UserId.
Update-MgBetaUserMessage -UserId $userId -MessageId $messageId -BodyParameter $params

```