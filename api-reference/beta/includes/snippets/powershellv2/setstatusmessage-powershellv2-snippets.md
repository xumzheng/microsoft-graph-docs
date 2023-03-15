---
description: "Automatically generated file. DO NOT MODIFY"
---

```powershellv2

Import-Module Microsoft.Graph.Beta.Users.Actions

$params = @{
	StatusMessage = @{
		Message = @{
			Content = "Hey I'm currently in a meeting."
			ContentType = "text"
		}
		ExpiryDateTime = @{
			DateTime = "2022-10-18T17:05:33.2079781"
			TimeZone = "Pacific Standard Time"
		}
	}
}

Set-MgBetaUserPresenceStatusMessage -UserId $userId -BodyParameter $params

```