---
description: "Automatically generated file. DO NOT MODIFY"
---

```powershellv2

Import-Module Microsoft.Graph.Beta.Users.Actions

$params = @{
	availability = "DoNotDisturb"
	activity = "DoNotDisturb"
	expirationDuration = "PT8H"
}

Set-MgBetaUserPresenceUserPreferredPresence -UserId $userId -BodyParameter $params

```