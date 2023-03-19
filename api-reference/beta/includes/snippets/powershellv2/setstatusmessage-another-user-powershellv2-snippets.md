---
description: "Automatically generated file. DO NOT MODIFY"
---

```powershellv2

Import-Module Microsoft.Graph.Beta.Users.Actions

$params = @{
	StatusMessage = @{
		Message = @{
			Content = "Hey I am available now"
			ContentType = "text"
		}
	}
}

Set-MgBetaUserPresenceStatusMessage -UserId $userId -BodyParameter $params

```