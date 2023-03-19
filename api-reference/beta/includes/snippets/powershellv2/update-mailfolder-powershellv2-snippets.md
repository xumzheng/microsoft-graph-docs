---
description: "Automatically generated file. DO NOT MODIFY"
---

```powershellv2

Import-Module Microsoft.Graph.Beta.Mail

$params = @{
	DisplayName = "displayName-value"
}

# A UPN can also be used as -UserId.
Update-MgBetaUserMailFolder -UserId $userId -MailFolderId $mailFolderId -BodyParameter $params

```