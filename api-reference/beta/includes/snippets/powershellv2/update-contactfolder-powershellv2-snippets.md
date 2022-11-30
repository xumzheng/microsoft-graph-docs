---
description: "Automatically generated file. DO NOT MODIFY"
---

```powershellv2

Import-Module Microsoft.Graph.Beta.PersonalContacts

$params = @{
	ParentFolderId = "parentFolderId-value"
	DisplayName = "displayName-value"
}

# A UPN can also be used as -UserId.
Update-MgBetaUserContactFolder -UserId $userId -ContactFolderId $contactFolderId -BodyParameter $params

```