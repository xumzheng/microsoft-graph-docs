---
description: "Automatically generated file. DO NOT MODIFY"
---

```powershellv2

Import-Module Microsoft.Graph.CloudCommunications

$params = @{
	Role = "viewer"
}

Rename-MgCommunicationCallScreenSharingRole -CallId $callId -BodyParameter $params

```