---
description: "Automatically generated file. DO NOT MODIFY"
---

```powershellv2

Import-Module Microsoft.Graph.Beta.Files

$params = @{
	recipients = @(
		@{
			email = "john@contoso.com"
		}
		@{
			email = "ryan@external.com"
		}
	)
	roles = @(
		"read"
	)
}

Grant-MgBetaSharesPermission -SharedDriveItemId $sharedDriveItemId -BodyParameter $params

```