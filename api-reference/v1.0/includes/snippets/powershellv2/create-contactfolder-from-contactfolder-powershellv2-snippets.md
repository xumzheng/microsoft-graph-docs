---
description: "Automatically generated file. DO NOT MODIFY"
---

```powershellv2

Import-Module Microsoft.Graph.PersonalContacts

$params = @{
	displayName = "Family"
}

# A UPN can also be used as -UserId.
New-MgUserContactFolderChildFolder -UserId $userId -ContactFolderId $contactFolderId -BodyParameter $params

```