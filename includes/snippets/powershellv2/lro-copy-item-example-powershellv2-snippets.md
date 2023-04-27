---
description: "Automatically generated file. DO NOT MODIFY"
---

```powershellv2

Import-Module Microsoft.Graph.Beta.Files

$params = @{
	parentReference = @{
		path = "/drive/root:/Documents"
	}
	name = "Copy of LargeFolder1"
}

Copy-MgBetaDrivesItem -DriveId $driveId -DriveItemId $driveItemId -BodyParameter $params

```