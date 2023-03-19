---
description: "Automatically generated file. DO NOT MODIFY"
---

```powershellv2

Import-Module Microsoft.Graph.Beta.CloudCommunications

$params = @{
	TransferTarget = @{
		EndpointType = "default"
		Identity = @{
			User = @{
				Id = "550fae72-d251-43ec-868c-373732c2704f"
				TenantId = "72f988bf-86f1-41af-91ab-2d7cd011db47"
				DisplayName = "Heidi Steen"
			}
		}
		LanguageId = "languageId-value"
		Region = "region-value"
	}
}

Move-MgBetaCommunicationsCall -CallId $callId -BodyParameter $params

```