---
description: "Automatically generated file. DO NOT MODIFY"
---

```powershell

Import-Module Microsoft.Graph.Files

$params = @{
	ParentReference = @{
		Id = "String"
	}
	Name = "String"
}

Restore-MgDriveItem -DriveId $driveId -DriveItemId $driveItemId -BodyParameter $params

```