---
description: "Automatically generated file. DO NOT MODIFY"
---

```powershellv2

Import-Module Microsoft.Graph.Beta.CloudCommunications

$params = @{
	ClientContext = "d45324c1-fcb5-430a-902c-f20af696537c"
}

Invoke-MgBetaMuteCommunicationCallParticipant -CallId $callId -ParticipantId $participantId -BodyParameter $params

```