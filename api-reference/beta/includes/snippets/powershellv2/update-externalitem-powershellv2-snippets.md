---
description: "Automatically generated file. DO NOT MODIFY"
---

```powershellv2

Import-Module Microsoft.Graph.Beta.Search

$params = @{
	Acl = @(
		@{
			Type = "everyone"
			Value = "67a141d8-cf4e-4528-ba07-bed21bfacd2d"
			AccessType = "grant"
		}
	)
}

Update-MgBetaExternalConnectionItem -ExternalConnectionId $externalConnectionId -ExternalItemId $externalItemId -BodyParameter $params

```