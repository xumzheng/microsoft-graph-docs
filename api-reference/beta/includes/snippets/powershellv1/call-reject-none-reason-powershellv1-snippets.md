---
description: "Automatically generated file. DO NOT MODIFY"
---

```powershellv1

Import-Module Microsoft.Graph.CloudCommunications

$params = @{
	Reason = "none"
}

Invoke-MgRejectCommunicationCall -CallId $callId -BodyParameter $params

```