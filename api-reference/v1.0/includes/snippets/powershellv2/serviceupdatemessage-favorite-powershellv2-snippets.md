---
description: "Automatically generated file. DO NOT MODIFY"
---

```powershellv2

Import-Module Microsoft.Graph.Devices.ServiceAnnouncement

$params = @{
	messageIds = @(
		"MC172851"
		"MC167983"
	)
}

Invoke-MgFavoriteServiceAnnouncementMessage -BodyParameter $params

```