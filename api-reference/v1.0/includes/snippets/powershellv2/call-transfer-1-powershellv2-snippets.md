---
description: "Automatically generated file. DO NOT MODIFY"
---

```powershellv2

Import-Module Microsoft.Graph.CloudCommunications

$params = @{
	TransferTarget = @{
		EndpointType = "default"
		Identity = @{
			User = @{
				Id = "550fae72-d251-43ec-868c-373732c2704f"
				DisplayName = "Heidi Steen"
			}
		}
	}
}

Move-MgCommunicationsCall -CallId $callId -BodyParameter $params

```