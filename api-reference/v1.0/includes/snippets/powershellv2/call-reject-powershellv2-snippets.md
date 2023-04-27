---
description: "Automatically generated file. DO NOT MODIFY"
---

```powershellv2

Import-Module Microsoft.Graph.CloudCommunications

$params = @{
	reason = "busy"
}

Invoke-MgRejectCommunicationCall -CallId $callId -BodyParameter $params

```