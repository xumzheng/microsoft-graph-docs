---
description: "Automatically generated file. DO NOT MODIFY"
---

```powershellv2

Import-Module Microsoft.Graph.CloudCommunications

$params = @{
	reason = "none"
}

Invoke-MgRejectCommunicationCall -CallId $callId -BodyParameter $params

```