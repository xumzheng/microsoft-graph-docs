---
description: "Automatically generated file. DO NOT MODIFY"
---

```powershellv2

Import-Module Microsoft.Graph.Beta.CloudCommunications

$params = @{
	TransferTarget = @{
		EndpointType = "default"
		Identity = @{
			Phone = @{
				"@odata.type" = "#microsoft.graph.identity"
				Id = "+12345678901"
			}
		}
		LanguageId = "languageId-value"
		Region = "region-value"
	}
}

Move-MgBetaCommunicationsCall -CallId $callId -BodyParameter $params

```