---
description: "Automatically generated file. DO NOT MODIFY"
---

```powershellv2

Import-Module Microsoft.Graph.Users.Actions

$params = @{
	availability = "DoNotDisturb"
	activity = "DoNotDisturb"
	expirationDuration = "PT8H"
}

Set-MgUserPresenceUserPreferredPresence -UserId $userId -BodyParameter $params

```