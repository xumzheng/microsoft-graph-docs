---
description: "Automatically generated file. DO NOT MODIFY"
---

```powershellv2

Import-Module Microsoft.Graph.Beta.CloudCommunications

$params = @{
	Participants = @(
		""
	)
	ClientContext = "clientContext-value"
}

Invoke-MgBetaMuteAllCommunicationCallParticipant -CallId $callId -BodyParameter $params

```