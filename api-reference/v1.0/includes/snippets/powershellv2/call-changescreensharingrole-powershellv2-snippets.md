---
description: "Automatically generated file. DO NOT MODIFY"
---

```powershellv2

Import-Module Microsoft.Graph.CloudCommunications

$params = @{
	role = "viewer"
}

Rename-MgCommunicationCallScreenSharingRole -CallId $callId -BodyParameter $params

```