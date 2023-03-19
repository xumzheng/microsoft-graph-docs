---
description: "Automatically generated file. DO NOT MODIFY"
---

```powershellv2

Import-Module Microsoft.Graph.Users.Actions

$params = @{
	DestinationId = "destinationId-value"
}

# A UPN can also be used as -UserId.
Move-MgUsersMailFolder -UserId $userId -MailFolderId $mailFolderId -BodyParameter $params

```