---
description: "Automatically generated file. DO NOT MODIFY"
---

```powershellv2

Import-Module Microsoft.Graph.Beta.CloudCommunications

$params = @{
	Reason = "none"
}

Invoke-MgBetaRejectCommunicationCall -CallId $callId -BodyParameter $params

```