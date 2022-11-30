---
description: "Automatically generated file. DO NOT MODIFY"
---

```powershellv2

Import-Module Microsoft.Graph.Beta.Users.Actions

$params = @{
	Availability = "DoNotDisturb"
	Activity = "DoNotDisturb"
	ExpirationDuration = "PT8H"
}

Set-MgBetaUserPresenceUserPreferredPresence -UserId $userId -BodyParameter $params

```