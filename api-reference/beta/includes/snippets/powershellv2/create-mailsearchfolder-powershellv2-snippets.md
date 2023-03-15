---
description: "Automatically generated file. DO NOT MODIFY"
---

```powershellv2

Import-Module Microsoft.Graph.Beta.Mail

$params = @{
	"@odata.type" = "microsoft.graph.mailSearchFolder"
	DisplayName = "Weekly digests"
	IncludeNestedFolders = $true
	SourceFolderIds = @(
		"AQMkADYAAAIBDAAAAA=="
	)
	FilterQuery = "contains(subject, 'weekly digest')"
}

# A UPN can also be used as -UserId.
New-MgBetaUserMailFolderChildFolder -UserId $userId -MailFolderId $mailFolderId -BodyParameter $params

```