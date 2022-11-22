---
description: "Automatically generated file. DO NOT MODIFY"
---

```powershellv2

Import-Module Microsoft.Graph.Beta.CloudCommunications

$params = @{
	BargeInAllowed = $true
	ClientContext = "d45324c1-fcb5-430a-902c-f20af696537c"
	Prompts = @(
		@{
			"@odata.type" = "#microsoft.graph.mediaPrompt"
		}
	)
	MaxRecordDurationInSeconds = 10
	InitialSilenceTimeoutInSeconds = 5
	MaxSilenceTimeoutInSeconds = 2
	PlayBeep = $true
	StopTones = @(
		"#"
		"1"
		"*"
	)
}

Invoke-MgBetaRecordCommunicationCallResponse -CallId $callId -BodyParameter $params

```