---
description: "Automatically generated file. DO NOT MODIFY"
---

```powershellv2

Import-Module Microsoft.Graph.Beta.PersonalContacts

$params = @{
	ParentFolderId = "parentFolderId-value"
	Birthday = [System.DateTime]::Parse("2016-10-19T10:37:00Z")
	FileAs = "fileAs-value"
	DisplayName = "displayName-value"
	GivenName = "givenName-value"
	Initials = "initials-value"
}

# A UPN can also be used as -UserId.
New-MgBetaUserContactFolderContact -UserId $userId -ContactFolderId $contactFolderId -BodyParameter $params

```