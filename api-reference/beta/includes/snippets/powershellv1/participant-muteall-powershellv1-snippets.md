---
description: "Automatically generated file. DO NOT MODIFY"
---

```powershellv1

Import-Module Microsoft.Graph.CloudCommunications

$params = @{
	Participants = @(
		""
	)
	ClientContext = "clientContext-value"
}

Invoke-MgMuteAllCommunicationCallParticipant -CallId $callId -BodyParameter $params

```