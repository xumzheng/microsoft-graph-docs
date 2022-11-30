---
description: "Automatically generated file. DO NOT MODIFY"
---

```powershellv2

Import-Module Microsoft.Graph.Beta.Mail

$params = @{
	DisplayName = "displayName-value"
	IsHidden = $true
}

# A UPN can also be used as -UserId.
New-MgBetaUserMailFolderChildFolder -UserId $userId -MailFolderId $mailFolderId -BodyParameter $params

```