---
description: "Automatically generated file. DO NOT MODIFY"
---

```powershellv2

Import-Module Microsoft.Graph.Users.Actions

$params = @{
	DestinationId = "deleteditems"
}

# A UPN can also be used as -UserId.
Move-MgUsersMessage -UserId $userId -MessageId $messageId -BodyParameter $params

```