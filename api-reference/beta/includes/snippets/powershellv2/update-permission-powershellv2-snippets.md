---
description: "Automatically generated file. DO NOT MODIFY"
---

```powershellv2

Import-Module Microsoft.Graph.Beta.Files

$params = @{
	roles = @(
		"read"
	)
}

Update-MgBetaDriveItemPermission -DriveId $driveId -DriveItemId $driveItemId -PermissionId $permissionId -BodyParameter $params

```