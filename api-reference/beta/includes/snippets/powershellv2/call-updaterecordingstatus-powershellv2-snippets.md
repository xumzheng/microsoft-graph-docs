---
description: "Automatically generated file. DO NOT MODIFY"
---

```powershellv2

Import-Module Microsoft.Graph.Beta.CloudCommunications

$params = @{
	ClientContext = "clientContext-value"
	Status = "notRecording | recording | failed"
}

Update-MgBetaCommunicationCallRecordingStatus -CallId $callId -BodyParameter $params

```