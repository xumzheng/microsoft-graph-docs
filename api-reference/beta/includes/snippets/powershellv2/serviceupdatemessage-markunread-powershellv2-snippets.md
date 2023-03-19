---
description: "Automatically generated file. DO NOT MODIFY"
---

```powershellv2

Import-Module Microsoft.Graph.Beta.Devices.ServiceAnnouncement

$params = @{
	MessageIds = @(
		"MC172851"
		"MC167983"
	)
}

Invoke-MgBetaMarkServiceAnnouncementMessageUnread -BodyParameter $params

```