---
description: "Automatically generated file. DO NOT MODIFY"
---

```powershellv2

Import-Module Microsoft.Graph.Beta.Users.Actions

$params = @{
	DestinationId = "deleteditems"
}

# A UPN can also be used as -UserId.
Move-MgBetaUsersMessage -UserId $userId -MessageId $messageId -BodyParameter $params

```