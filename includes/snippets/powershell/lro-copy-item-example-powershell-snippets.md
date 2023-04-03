---
description: "Automatically generated file. DO NOT MODIFY"
---

```powershell

Import-Module Microsoft.Graph.Files

$params = @{
	ParentReference = @{
		Path = "/drive/root:/Documents"
	}
	Name = "Copy of LargeFolder1"
}

Copy-MgDriveItem -DriveId $driveId -DriveItemId $driveItemId -BodyParameter $params

```