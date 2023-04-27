---
description: "Automatically generated file. DO NOT MODIFY"
---

```powershellv2

Import-Module Microsoft.Graph.Files

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

Grant-MgSharesPermission -SharedDriveItemId $sharedDriveItemId -BodyParameter $params

```