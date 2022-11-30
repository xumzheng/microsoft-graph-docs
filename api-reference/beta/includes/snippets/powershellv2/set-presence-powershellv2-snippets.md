---
description: "Automatically generated file. DO NOT MODIFY"
---

```powershellv2

Import-Module Microsoft.Graph.Beta.Users.Actions

$params = @{
	SessionId = "22553876-f5ab-4529-bffb-cfe50aa89f87"
	Availability = "Available"
	Activity = "Available"
	ExpirationDuration = "PT1H"
}

Set-MgBetaUserPresence -UserId $userId -BodyParameter $params

```