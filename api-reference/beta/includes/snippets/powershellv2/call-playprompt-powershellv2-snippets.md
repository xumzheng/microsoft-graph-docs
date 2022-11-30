---
description: "Automatically generated file. DO NOT MODIFY"
---

```powershellv2

Import-Module Microsoft.Graph.Beta.CloudCommunications

$params = @{
	ClientContext = "d45324c1-fcb5-430a-902c-f20af696537c"
	Prompts = @(
		@{
			"@odata.type" = "#microsoft.graph.mediaPrompt"
			MediaInfo = @{
				"@odata.type" = "#microsoft.graph.mediaInfo"
				Uri = "https://cdn.contoso.com/beep.wav"
				ResourceId = "1D6DE2D4-CD51-4309-8DAA-70768651088E"
			}
		}
	)
	Loop = $false
}

Invoke-MgBetaPlayCommunicationCallPrompt -CallId $callId -BodyParameter $params

```