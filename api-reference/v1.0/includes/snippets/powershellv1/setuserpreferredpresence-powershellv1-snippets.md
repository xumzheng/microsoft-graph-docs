---
description: "Automatically generated file. DO NOT MODIFY"
---

```powershellv1

Import-Module Microsoft.Graph.Users.Actions

$params = @{
	Availability = "DoNotDisturb"
	Activity = "DoNotDisturb"
	ExpirationDuration = "PT8H"
}

Set-MgUserPresenceUserPreferredPresence -UserId $userId -BodyParameter $params

```