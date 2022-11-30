---
description: "Automatically generated file. DO NOT MODIFY"
---

```powershellv2

Import-Module Microsoft.Graph.Beta.Mail

$params = @{
	DisplayName = "Important from partner"
	Actions = @{
		MarkImportance = "high"
	}
}

# A UPN can also be used as -UserId.
Update-MgBetaUserMailFolderMessageRule -UserId $userId -MailFolderId $mailFolderId -MessageRuleId $messageRuleId -BodyParameter $params

```