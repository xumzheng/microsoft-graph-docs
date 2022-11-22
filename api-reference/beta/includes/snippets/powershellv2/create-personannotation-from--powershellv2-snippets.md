---
description: "Automatically generated file. DO NOT MODIFY"
---

```powershellv2

Import-Module Microsoft.Graph.Beta.People

$params = @{
	Detail = @{
		ContentType = "text"
		Content = "I am originally from Australia, but grew up in Moscow, Russia."
	}
	DisplayName = "About Me"
}

# A UPN can also be used as -UserId.
New-MgBetaUserProfileNote -UserId $userId -BodyParameter $params

```